# CSS
Code of CSS Web Development
*************************************************************************************************************************************************************************@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@700&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing:border-box;
    font-family: 'Poppins',sans-serif; 
    /*background-image: url(pic2.jpg);
    background-size: center;*/
}

body {
    background: #000000;
    background-image: url(pic33.jpg);
    background-size: cover;
    
}

.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 25px 12.5%;
    background: transparent;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100; 
}

.navbar a {
    position: relative;
    font-size: 16px;
    color:#e4e4e4;
    text-decoration: none;
    font-weight: 500;
    margin-right: 30px;
}

.navbar a::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: -6px;
    width: 100%;
    height: 2px;
    background: #e4e4e4;
    border-radius: 5px;
   /* transform-origin: right;*/
    transform: scaleX(0);
    transform: transform .5s;
   /* transform: translateY(10px);
    opacity: 0;
    transition: .5s;*/
}

.navbar a:hover::after {
    /*transform: translateY(0);
    opacity: 1;*/
    transform: scaleX(1);
}

.search-bar {
    width: 250px;
    height: 45px;
    background: transparent;
    border: 2px solid #e4e4e4;
    border-radius: 6px;
    display:flex;
    align-items: centre;
}

.search-bar input {
    width: 100%;
    background: transparent;
    border: none;
    outline: none;
    font-size: 16px;
    color:#e4e4e4;
    padding-left: 10px;
}

.search-bar input::placeholder {
    color:#e4e4e4;
}

.search-bar button {
    width: 40px;
    height: 100%;
    background: transparent;
    border: none;
    outline: none;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
}

.search-bar button i {
    font-size: 22px;
    color: #e4e4e4;
}

.container {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 75%;
    height: 550px;
    background: url('pic16.jpg') no-repeat;
    background-size: cover;
    background-position: cover;
    margin-top: 20px;

}

.container .content {
    position: absolute;
    top: 0;
    left: 0;
    width: 58;
    height: 100%;
    background: transparent;
    padding: 80px; 
    color: #e4e4e4;
    display: flex;
    justify-content: space-between;
    flex-direction: column;

}

.content .logo {
    font-size: 30px;
}

.text-sci h2 {
    font-size: 40px;
    line-height: 1; 
}

.text-sci h2 span {
    font-size: 25px;
}

.text-sci p{
    font-size:16px;
    margin:20px 0;
}

.social-icons a i {
    font-size:22px;
    color: white;
    margin-right: 10px;
    transition: .5s ease-in-out;
}

.social-icons a:hover i {
    transform: scale(1.2);
}




.container .logreg-box{
    position:absolute;
    top: 0;
    right: 0;
    width: calc(100% - 58%);
    height: 100%;
    overflow:hidden;
}


.logreg-box .form-box {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
    background: transparent;
    backdrop-filter: blur(20px);
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
    color: #e4e4e4;

}

.logreg-box .form-box.login{
    transform: translateX(0);
    transition: transform .6s ease;
    transition-delay: .7s;
}

.logreg-box.active .form-box.login{
    transform: translate(430px);
    transition-delay: 0s;
}
.logreg-box .form-box.register{
    transform: translateX(430px);
    transition: transform .6s ease;
    transition-delay: 0s;
}

.logreg-box.active .form-box.register{
    transform: translateX(0);
    transition-delay: .7s;
}

.form-box h2{
    font-size:32px;
    text-align: center;
}

.form-box .input-box{
    position: relative;
    width:340px;
    height: 50px;
    border-bottom: 2px solid #e4e4e4;
    margin: 30px 0;
}

.input-box input{
    width: 100%;
    height: 100%;
    background: transparent;
    border: none;
    outline: none;
    font-size: 16px;
    color:#e4e4e4;
    font-weight: 500;
    padding-right: 28px;
}

.input-box label{
    position: absolute;
    top: 50%;
    left: 0;
    transform: translateY(-50%);
    font-size: 16px;
    font-weight: 500;
    pointer-events: none;
    transition: 0.5s ease;
}

.input-box input:focus~label,
.input-box input:valid~label {
    top: -5px;
}
.input-box .icon{
    position: absolute;
    top: 13px;
    right: 0;
    font-size: 19px;
}

.form-box .remember-forgot {
    font-size: 14.5px;
    font-weight: 500;
    margin: -15px 0 15px;
    display:flex;
    justify-content: space-between;
}

.remember-forgot label input {
    accent-color: #e4e4e4;
    margin-right: 3px;
}

.remember-forgot a {
    color: #e4e4e4;
    text-decoration: none;
}

.remember-forgot a:hover {
    text-decoration: underline;
}

.navbar .Login {
    width: 100px;
    height: 40px;
    background: transparent;
    border: 2px solid #fff;
    outline: none;
    border-radius: 10px;
    cursor: pointer;
    font-size: 1.1em;
    color: #fff;
    font-weight: 50;
    margin-right: 275px;
    transition: .5s;

}
.navbar .Login:hover {
    background: #e4e4e4;
    color: #162938;
}

.btn {
    width: 100%;
    height: 45px;
    background: #c4103d00;
    border: none;
    outline: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
    color: #020410;
    font-weight: 500;
    box-shadow: 0 0 10px rgba(0, 0, 0, .5);
}

.form-box .login-register {
    font-size: 14.5px;
    font-weight: 500;
    text-align: center;
    margin-top: 25px;
}

.login-register p a {
    color: #e4e4e4;
    font-weight: 600;
    text-decoration: none;
}

.login-register p a:hover{
    text-decoration: underline;
}


