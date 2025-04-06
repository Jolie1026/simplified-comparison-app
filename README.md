# 图片对比应用 (Image Comparison App)

这是一个简单易用的Web应用程序，允许用户上传两张图片并进行交互式对比或生成动态GIF。它非常适合展示“前后”变化，例如城市发展、环境变迁、项目进展等。

## 功能

*   **交互式滑块对比**: 上传两张图片后，可以通过拖动滑块直观地比较两张图片的差异。
*   **动态GIF生成**: 自动创建在两张图片之间平滑切换（划像效果）的动画GIF。
*   **自定义标签**: 为每张图片添加标签（例如，年份、版本号），标签会显示在对比滑块和生成的GIF上。
*   **标签样式调整**: 可以选择不同的标签背景颜色和文字颜色。
*   **GIF过渡速度调整**: 可以自定义GIF中两张图片切换的速度。
*   **响应式设计**: 在不同设备上都能良好显示。
*   **纯前端实现**: 所有处理都在用户的浏览器中完成，无需服务器端支持，保护用户隐私。
*   **拖放上传**: 支持直接将图片拖放到上传区域。
*   **本地运行**: 只需下载 `simplified-comparison-app.html` 和 `gif.worker.js` 文件，用浏览器打开 `simplified-comparison-app.html` 即可使用。

## 如何使用 (How to Use / 사용 방법)

### 中文 (Chinese)
1.  **下载文件**:
    *   下载 `simplified-comparison-app.html` 文件。
    *   下载 `gif.worker.js` 文件。**确保这两个文件放在同一个文件夹下**。
2.  **启动Web服务**:
    *   由于浏览器安全限制，直接打开HTML文件可能无法正常工作，需要通过Web服务器访问。
    *   您可以使用以下任一方法启动本地Web服务:
        *   Python: 在文件所在目录运行 `python -m http.server`
        *   Node.js: 安装 `http-server` 后运行 `http-server`
        *   VSCode: 使用 "Live Server" 扩展
        *   其他: 使用XAMPP、WAMP或任何其他Web服务器
3.  **打开应用**: 通过浏览器访问本地Web服务提供的URL(通常是 `http://localhost:8000` 或类似地址)。
4.  **上传图片**:
    *   点击左侧的“选择图片”按钮或将图片拖放到左侧区域，上传第一张图片（通常是“之前”或左侧的图片）。
    *   点击右侧的“选择图片”按钮或将图片拖放到右侧区域，上传第二张图片（通常是“之后”或右侧的图片）。
    *   **建议**: 为了获得最佳效果，请上传两张**尺寸相同**的图片。如果尺寸不同，GIF生成时会自动裁剪为两张图片中较小的尺寸。
5.  **添加标签 (可选)**: 在图片下方的输入框中为每张图片输入标签，例如 "2010年" 和 "2024年"。

### English
1.  **Download Files**:
    *   Download the `simplified-comparison-app.html` file.
    *   Download the `gif.worker.js` file. **Ensure both files are in the same folder**.
2.  **Start a Web Server**:
    *   Due to browser security restrictions, opening the HTML file directly may not work. Access it via a web server.
    *   You can use any of the following methods to start a local web server:
        *   Python: Run `python -m http.server` in the directory containing the files.
        *   Node.js: Install `http-server` and run `http-server`.
        *   VSCode: Use the "Live Server" extension.
        *   Others: Use XAMPP, WAMP, or any other web server.
3.  **Open the App**: Access the app via the URL provided by the web server (usually `http://localhost:8000` or similar).
4.  **Upload Images**:
    *   Click the "Select Image" button on the left or drag and drop an image into the left area to upload the first image (usually the "before" or left image).
    *   Click the "Select Image" button on the right or drag and drop an image into the right area to upload the second image (usually the "after" or right image).
    *   **Recommendation**: For best results, upload two images of the **same size**. If the sizes differ, the GIF will be cropped to the smaller image's dimensions.
5.  **Add Labels (Optional)**: Enter labels for each image in the input fields below the images, e.g., "2010" and "2024".

### 한국어 (Korean)
1.  **파일 다운로드**:
    *   `simplified-comparison-app.html` 파일을 다운로드하세요.
    *   `gif.worker.js` 파일을 다운로드하세요. **두 파일이 동일한 폴더에 있는지 확인하세요**.
2.  **웹 서버 시작**:
    *   브라우저 보안 제한으로 인해 HTML 파일을 직접 열면 작동하지 않을 수 있습니다. 웹 서버를 통해 액세스하세요.
    *   로컬 웹 서버를 시작하려면 다음 방법 중 하나를 사용할 수 있습니다:
        *   Python: 파일이 있는 디렉토리에서 `python -m http.server` 명령을 실행하세요.
        *   Node.js: `http-server`를 설치한 후 `http-server` 명령을 실행하세요.
        *   VSCode: "Live Server" 확장을 사용하세요.
        *   기타: XAMPP, WAMP 또는 다른 웹 서버를 사용하세요.
3.  **앱 열기**: 웹 서버에서 제공하는 URL(일반적으로 `http://localhost:8000` 또는 유사한 주소)을 통해 앱에 액세스하세요.
4.  **이미지 업로드**:
    *   왼쪽의 "이미지 선택" 버튼을 클릭하거나 이미지를 왼쪽 영역으로 드래그 앤 드롭하여 첫 번째 이미지를 업로드하세요(일반적으로 "이전" 또는 왼쪽 이미지).
    *   오른쪽의 "이미지 선택" 버튼을 클릭하거나 이미지를 오른쪽 영역으로 드래그 앤 드롭하여 두 번째 이미지를 업로드하세요(일반적으로 "이후" 또는 오른쪽 이미지).
    *   **권장 사항**: 최상의 결과를 얻으려면 **동일한 크기**의 두 이미지를 업로드하세요. 크기가 다르면 GIF는 더 작은 이미지의 크기로 잘립니다.
5.  **레이블 추가 (선택 사항)**: 이미지 아래의 입력 필드에 각 이미지의 레이블을 입력하세요(예: "2010년" 및 "2024년").

## 技术栈

*   HTML5
*   CSS3
*   JavaScript (原生)
*   [gif.js](https://github.com/jnordberg/gif.js) (用于GIF编码，已包含 `gif.worker.js`)
*   [Font Awesome](https://fontawesome.com/) (用于图标)

## 贡献

欢迎提出改进建议或报告问题！您可以通过 GitHub Issues 来提交。

## 许可

本项目采用 [MIT 许可证](LICENSE)。