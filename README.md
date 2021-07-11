<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>form</title>
    <link rel="stylesheet" href="./assets/css/base.css">
	<link rel="stylesheet" href="./assets/css/main.css">
	<link rel="stylesheet" href="./assets/fonts/fontawesome-free-5.15.3-web/css/all.min.css">
	
</head>
<body>
    <div class="main">
        <form action="" method="post" id="form-1">
            <div class="auth-form__form">
                <div class="auth-form">
                        
                    <div class="auth-form_container">
                        <div class="auth-form_header">
                            <h3 class="auth-form_heading">Đăng ký</h3>
                            <span class="auth-form_login">Đăng nhập</span>
                        </div>
                        <div class="auth-form__form ">
                            <div class="auth-form__group ">
                                <input id="fullname" name="name" type="text" class="auth-form__input" placeholder="User">
                                <span class="form_message"></span>
                            </div>
                            <div class="auth-form__group invalid">
                                <input id="email" name="email" type="text" class="auth-form__input" placeholder="Email">
                                <span class="form_message"></span>
                            </div>
                            <div class="auth-form__group">
                                <input id="pass" name="password" type="text" class="auth-form__input" placeholder="Password">
                                <span class="form_message"></span>
                            </div>
                            <div class="auth-form__group">
                                <input id="confirm" name="password_confirm  " type="text" class="auth-form__input" placeholder="Password confirm">
                                <span class="form_message"></span>
                            </div>
                        </div>
                        <div class="auth-form__aside">
                            <p class="auth-form__chinhsach-text">Bằng việc đăng kí, bạn đã đồng ý với Shopee về
                                <a href="" class="auth-form__link">Điều khoản và dịch vụ</a> &
                                <a href="" class="auth-form__link">Chính sách bảo mật</a>
                            </p>
                        </div>
                        <div class="auth-form__control">
                            <button type="submit" class="btn btn--primary">ĐĂNG KÝ</button>
                        </div>
                    </div>
                    <!-- <div class="auth-form__socials">
                        
                            <a href="" class="btn btn_size--s btn--with_icon-fb">
                                <i class=" auth-form__socials--icon fab fa-facebook-square"></i>
                                <span class="label">Kết nối với Facebook</span>
                            </a>
                            <a href="" class="btn btn_size--s btn--with_icon-gg">
                                <i class=" auth-form__socials--icon fab fa-google"></i>
                               <span class="label"> Kết nối với Google</span>
                            </a>
                    </div> -->
                </div>
            </div>
        </form>
    </div>
    <script src="./validate.js"></script>
    <script>
        Validate({
            form: '#form-1',
            rules: [
                Validate.isRequired('#fullname'),
                Validate.isEmail('#email'),
                Validate.isPass('#pass'),
                Validate.isConfirm('#confirm')
            ]
        });
    </script>
</body>
</html>
