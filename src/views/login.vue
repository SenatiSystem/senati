<template>
    <div>
        <section>
        <div class="imgBx">
            <img src="../assets/senati_login.jpg" alt="">
        </div>
        <div class="contentBx">

            <div class="formBx">
                <h2>Iniciar Sesion</h2>
                <form>
                    <div class="inputBx">
                        <span>Usuario</span>
                        <input type="text" name="">
                    </div>
                    <div class="inputBx">
                        <span>Contraseña</span>
                        <input type="password" name="">
                    </div>
                    <div class="remember">
                        <label><input type="checkbox" name="">Recordar Contraseña</label>
                    </div>
                    <div class="inputBx">
                        <input type="submit" value="Iniciar Sesion" name="">
                    </div>

                </form>
                <h3>Ingresar a nuestras paginas</h3>
                <ul class="sci">
                    <li>
                        <a href="https://www.facebook.com/SenatiOficial/"><img src="../assets/facebook.png" alt="" style="width: 40px;height: 40px;"></a>
                    </li>
                    <li>
                        <a href="https://www.facebook.com/SenatiOficial/"><img src="../assets/youtube.png" alt="" style="width: 50px;height: 50px;"></a>

                    </li>
                </ul>
            </div>
        </div>
    </section>
    </div>
</template>

<script>
export default {
    name: 'Home'
}
</script>

<style scoped>
 @import url('https://fonts.googleapis.com/css2? family = Poppins: ital, wght @ 0,100; 0,200; 0,300; 0,400; 0,500; 0,600; 0,700; 0,800; 0,900; 1,100; 1,200; 1.300; 1.400; 1.500; 1.600; 1.700; 1.800; 1.900 & display = swap ');
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: 'Poppins', sans-serif;
    }
    
    section {
        position: relative;
        width: 100%;
        height: 100vh;
        display: flex;
    }
    
    section .imgBx {
        position: relative;
        width: 50%;
        height: 100%;
    }
    
    section .imgBx::before {
        position: absolute;
        content: '';
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(225deg, #0c3247, #03a9f4);
        z-index: 1;
        mix-blend-mode: screen;
    }
    
    section .imgBx img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    
    section .contentBx {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 50%;
        height: 100%;
    }
    
    section .contentBx .formBx {
        width: 50%;
    }
    
    section .contentBx .formBx h2 {
        color: #607d8b;
        font-weight: 600;
        font-size: 1.5em;
        text-transform: uppercase;
        margin-bottom: 20px;
        border-bottom: 4px solid #03a9f4;
        display: inline-block;
        letter-spacing: 1px;
    }
    
    section .contentBx .formBx .inputBx {
        margin-bottom: 20px;
    }
    
    section .contentBx .formBx .inputBx span {
        font-size: 16px;
        margin-bottom: 5px;
        display: inline-block;
        color: #607db8;
        font-weight: 300;
        font-size: 16px;
        letter-spacing: 1px;
    }
    
    section .contentBx .formBx .inputBx input {
        width: 100%;
        padding: 10px 20px;
        outline: none;
        font-weight: 400;
        border: 1px solid #607d8b;
        font-size: 16px;
        letter-spacing: 1px;
        color: #607d8b;
        background: transparent;
        border-radius: 30px;
    }
    
    section .contentBx .formBx .inputBx input[type="submit"] {
        background: #03a9f4;
        color: #fff;
        border: none;
        font-weight: 500;
        cursor: pointer;
    }
    
    section .contentBx .formBx .inputBx input[type="submit"]:hover {
        background: skyblue;
    }
    
    .remember {
        margin-bottom: 10px;
        color: #607d8b;
        font-weight: 400;
        font-size: 14px;
    }
    
    section .contentBx .formBx h3 {
        color: #607d8b;
        text-align: center;
        margin: 80px 0 10px;
        font-weight: 500;
    }
    
    section .contentBx .formBx .sci {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    
    section .contentBx .formBx .sci li {
        list-style: none;
        width: 50px;
        height: 50px;
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 0 7px;
    }
    
    @media (max-width:768px) {
        section .imgBx {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        section .contentBx {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 100%;
            height: 100%;
            z-index: 1;
        }
        section .contentBx .formBx {
            width: 100%;
            padding: 40px;
            background: rgb(255 255 255 / 0.9);
            margin: 50px;
        }
        section .contentBx .formBx h3 {
            color: #607d8b;
            text-align: center;
            margin: 30px 0 10px;
            font-weight: 500;
        }
    }
</style>