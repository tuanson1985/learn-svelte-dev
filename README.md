# learn-svelte

Tôi sử dụng repo này để theo dõi tất cả các bài học tôi đã học về `svelte`

## Tài liệu tham khảo

- https://svelte.dev/docs/introduction

- https://learn.svelte.dev/tutorial/welcome-to-svelte

## Công cụ playground trực tuyến

- https://svelte.dev/repl/hello-world?version=4.2.19

# Basic Svelte

## Introductuon

1. Welcometo Svelte

   - `Svelte` là gì? `Svelte` là một công cụ để xây dựng các ứng dụng web. Giống như các `framework` giao diện người dùng khác, `Svelte` cho phép bạn xây dựng ứng dụng của mình theo cách khai báo từ các thành phần kết hợp giữa đánh dấu, kiểu dáng và hành vi.

   - Các thành phần này được biên dịch thành các mô-đun `JavaScript` nhỏ gọn và hiệu quả, loại bỏ các chi phí bổ sung thường gắn liền với các `framework` giao diện người dùng.

   - Bạn có thể xây dựng toàn bộ ứng dụng của mình bằng `Svelte` (ví dụ, sử dụng một `framework` ứng dụng như `SvelteKit`, sẽ được đề cập trong hướng dẫn này), hoặc bạn có thể bổ sung `Svelte` vào một mã nguồn hiện có từng bước một. Bạn cũng có thể phát hành các thành phần như các gói độc lập hoạt động ở mọi nơi.

   - Cách sử dụng hướng dẫn này Bạn sẽ cần có kiến thức cơ bản về `HTML`, `CSS` và `JavaScript` để hiểu `Svelte`.

   - Hướng dẫn này được chia thành bốn phần chính:

     - `Basic Svelte` (Bạn đang ở đây).

     - `Advanced Svelte`.

     - `Basic SvelteKit`.

     - `Advanced SvelteKit`.

   - Khởi tạo dự án.

   ```svelte
   npm create svelte@latest myapp cd myapp npm install npm run dev
   ```

2. Your firt component.

   - Trong `Svelte`, một ứng dụng được tạo thành từ một hoặc nhiều thành phần `(components)`. Một thành phần là một khối mã tự chứa có thể tái sử dụng, bao gồm `HTML`, `CSS` và `JavaScript` liên quan, được viết trong một tệp `.svelte`. Tệp `App.svelte`, đang mở trong trình soạn thảo mã bên phải, là một thành phần đơn giản.

   ```svelte
   <script>
   	let name = 'Svelte';
   </script>

   <h1>Hello {name.toUpperCase()}!</h1>
   ```

3. Dynamic attributes
