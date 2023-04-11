# Hướng dẫn cài đặt và sử dụng Excel Add-ins ExcelTranslate AI

ExcelTranslate AI là một excel add-ins giúp bạn dịch một đoạn văn bản trong (các) cell bạn đang chọn trực tiếp trong file Excel mà không cần copy nội dung và đưa vào các công cụ dịch thuât khác
- Tác giả: Zedination
- Email: [leanhduc9999@gmail.com](mailto:leanhduc9999@gmail.com)
- Discord cá nhân: https://discordapp.com/users/958007722471719003

## Mục lục

- [Hướng dẫn cài đặt và sử dụng Excel Add-ins ExcelTranslate AI](#hướng-dẫn-cài-đặt-và-sử-dụng-excel-add-ins-exceltranslate-ai)
  - [Mục lục](#mục-lục)
  - [Tính năng](#tính-năng)
  - [Cài đặt](#cài-đặt)
  - [Cách sử dụng](#cách-sử-dụng)
  - [Một số lưu ý](#một-số-lưu-ý)
  - [License](#license)

## Tính năng
- Google Translate
- ChatGPT translate sử dụng reserve proxy server API (ChatGPT translate unoffical)
- ChatGPT translate sử dụng API cung cấp bởi OpenAI (ChatGPT translate offical)
- Bing AI Translate

## Cài đặt

1. Kiểm tra xem Ribbon Excel đã có tab **Developer** chưa hay chưa, nếu chưa được bật, hãy bật nó trong setting bằng cách truy cập **File** / **Options** / **Customize Ribbon** và tích vào checkbox **Developer**
   ![Screenshot 2023-04-12 001358](https://user-images.githubusercontent.com/50323429/231239582-fa34a45b-3fea-4f9e-a237-c45811455235.jpg)
2. Download ExcelTraslate AI [tại đây](https://zedination.dev/translate-ai/ExcelTranslate.xlam) và lưu vào một thư mục nhất định
3. Chọn vào tab **Developer**, sau đó chọn vào biểu tượng **Excel Add-ins** ![image](https://user-images.githubusercontent.com/50323429/231239955-d53bbc28-afd2-40b0-a234-0f31f92f7588.png), cửa sổ quản lý Add-ins của Excel hiện ra. Chọn button **Browse...** rồi chọn file **ExcelTranslate.xlam** mà bạn vừa download.

   ![image](https://user-images.githubusercontent.com/50323429/231241157-2360e51e-22d9-49cb-9d44-938b2259a82b.png)
4. Sau khi đã chọn file **ExcelTranslate.xlam**, cửa sổ quản lý add-ins sẽ xuất hiện mục **Exceltranslate**, hãy tích vào checkbox để kích hoạt Add-ins
5. Khởi động lại Excel và bắt đầu sử dụng thôi 😊

## Cách sử dụng
- Để sử dụng Google Translate, chọn vào cell cần dịch rồi bấm tổ hợp phím <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>T</kbd> hoặc <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Q</kbd>
  
  ![Animation](https://user-images.githubusercontent.com/50323429/231244062-16037a3f-c627-40ba-bb1f-f6b329dde797.gif)

- Trước khi có thể sử dụng ChatGPT dịch và Bing AI dịch thì phải config trước, để mở cửa sổ config hãy bấm tổ hợp phím <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Y</kbd>
    ![image](https://user-images.githubusercontent.com/50323429/231244677-31caad69-52fa-4209-a9d6-22cd1a7b9a12.png)
  - ChatGPT Access Token: input này dùng để nhập access_token cùa tài khoản ChatGPT của bạn, để lấy giá trị này hãy login tài khoản ChatGPT của bạn, sau đó truy cập [https://chat.openai.com/api/auth/session](https://chat.openai.com/api/auth/session), copy giá trị `accessToken` như hình dưới đây. Sau khi copy xong hãy nhập vào input **ChatGPT Access Token** rồi bấm <kbd>Save Config</kbd> tại cửa sổ config đang mở
    - <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/50323429/231246218-49541a26-405e-4939-b4f1-ccbfb90e2081.png">
      <img alt="NebulaGraph Data Intelligence Suite(ngdi)" src="https://user-images.githubusercontent.com/50323429/231246218-49541a26-405e-4939-b4f1-ccbfb90e2081.png">
    </picture>
    <!-- ![image](https://user-images.githubusercontent.com/50323429/231246218-49541a26-405e-4939-b4f1-ccbfb90e2081.png) -->
  - OpenAI API: truy cập [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys) để tạo API key cho riêng mình và nhập chúng vào đây
  - Bing Cookie _U: Truy cập Bing, sau đó đăng nhập tài khoản Microsoft của bạn rồi làm như trong ảnh sau để lấy cookie. Sau khi lấy cookies hãy nhập vào input Bing Cookie rồi bấm <kbd>Save Config</kbd> tại cửa sổ config đang mở để lưu cài đặt
    ![image](https://user-images.githubusercontent.com/50323429/231247618-d69e48aa-8484-48a5-bce8-803d457ab114.png)
  - Languages: Lựa chọn ngôn ngữ dịch đầu ra
  - Activated service: Lựa chọn trình dịch được sử dụng, mặc định sẽ là **Bing AI Translate**
  - Sau khi nhập xong các giá trị trên nhớ bấm <kbd>Save Config</kbd> tại cửa sổ config đang mở để lưu cài đặt nhé 😊
- Để sử dụng trình dịch AI, hãy chọn (các) cell cần dịch và bấm tổ hợp phím <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>X</kbd>. Tùy thuộc vào **Activated service** bạn đã config, trình dịch tương ứng sẽ được sử dụng. _Lưu ý: khi sử dụng trình dịch AI có thể phải chờ tương đối lâu để có kết quả dịch, hãy kiên nhẫn một chút nhé 😉_. Ví dụ trong ảnh dưới đây là kết quả khi sử dụng Bing AI Translate



  ![image](https://user-images.githubusercontent.com/50323429/231250513-d9b27d75-cd5a-4fda-90a3-ec5a45b97201.png)
  
## Một số lưu ý
- Đối với trình dịch là ChatGPT translate unoffical và Bing AI Translate, có thể hoạt động thiếu ổn định. Trong tương lai các dịch vụ này có thể không còn hỗ trợ nữa 😢
- Vui lòng không spam trong quá trình sử dụng để tránh các lỗi đáng tiếc có thể xảy ra
- Hãy ưu tiên sử dụng các service theo thứ tự ưu tiên như sau: Google Translate ->  Bing AI Translate -> ChatGPT translate offical -> ChatGPT translate unoffical. Hãy ưu tiên dịch bằng Google Translate, nếu không thể sử dụng Google Translate thì mới sử dụng các trình dịch AI khác

## License
This project is licensed under the MIT License

<blockquote>
Copyright (c) 2023 Zedination


Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
</blockquote>
