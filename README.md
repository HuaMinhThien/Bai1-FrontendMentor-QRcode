# Frontend Mentor - QR code component solution

This is a solution to the QR code component challenge on Frontend Mentor. Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

### Screenshot

![](./Screenshot%202025-08-30%20210551.png.jpg)

### Links

- Solution URL: [Add solution URL here](https://github.com/HuaMinhThien/Bai1-FrontendMentor-QRcode)
- Live Site URL: [Add live site URL here](https://huaminhthien.github.io/Bai1-FrontendMentor-QRcode/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS 3D Transforms
- Mobile-first workflow
- CSS Animations

### What I learned

Trong dự án này, tôi đã học được cách:
1. Sử dụng CSS Flexbox để căn giữa component một cách hoàn hảo
2. Tạo hiệu ứng 3D hover với CSS transforms và perspective
3. Sử dụng CSS animations với keyframes để tạo hiệu ứng màu sắc
4. Thiết kế responsive với min-width và max-width
5. Tạo bóng đổ với thuộc tính box-shadow

## Đoạn code CSS tôi tự hào:

```css
.container-card{
    background-color: hsl(0, 0%, 100%);
    width: 300px;
    min-height: 450px;  
    padding: 10px;
    border-radius: 10px;
    box-shadow: 5px 16px 10px #21212128;
    transition: transform 0.75s ease-in-out;
    transform: perspective(500px);
}

.container-card:hover{
    transform: perspective(500px) rotate3d(0, 2, -2, 6deg);
    animation: color-shift 1s ease-in-out infinite alternate;
}

@keyframes color-shift {
    0% {
        background: linear-gradient(45deg, #FFD700, #7CFC00);
    }
    25% {
        background: linear-gradient(45deg, #FFEC8B, #98FB98);
    }
    50% {
        background: linear-gradient(45deg, #FFFACD, #7CFC00);
    }
    75% {
        background: linear-gradient(45deg, #7CFC00, #FFD700);
    }
    100% {
        background: linear-gradient(45deg, #FFD700, #7CFC00);
    }
}
```

## Đoạn HTML structure tôi thiết kế:

```html
<div class="container-main">
    <div class="container-card">
      <div class="box1">
        <img src="images/image-qr-code.png" style="width: 100%; height: 100%; border-radius: 10px;" alt="">
      </div>
      <div class="box2">
        <div class="text1">
          <p>Improve your front-end skills by building projects</p>
        </div>
        <div class="text2">
          <p>Scan the QR code to visit Frontend</p>
          <p>Mentor and take your coding skills to the next level</p>
        </div>
      </div>
    </div>
  </div>
```

### Continued development

Trong các dự án tương lai, tôi muốn:
1. Tìm hiểu sâu hơn về CSS Grid để bố cục phức tạp hơn
2. Học thêm về CSS variables để quản lý màu sắc và kích thước hiệu quả hơn
3. Thử nghiệm với các hiệu ứng CSS nâng cao và transitions
4. Áp dụng phương pháp BEM (Block Element Modifier) cho đặt tên CSS class
5. Tối ưu hóa hiệu suất và khả năng truy cập (accessibility)

## Author

- Frontend Mentor - @Hữa Minh Thiện
- GitHub - Hữa Minh Thiện
- Facebook - [@Hua Minh Thien](https://www.facebook.com/minh.thien.460014/)
