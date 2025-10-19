<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>سوبر ماركت الحاضر | تسوق أونلاين</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    
    <style>
        /* الخطوط والأساسيات */
        :root {
            --primary-color: #4CAF50; /* أخضر زاهي */
            --secondary-color: #FFC107; /* أصفر مشرق */
            --accent-color: #2196F3; /* أزرق سماوي */
            --text-color: #333;
            --light-bg: #f8f9fa;
            --white: #ffffff;
            --dark-gray: #6c757d;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--light-bg);
            color: var(--text-color);
            line-height: 1.6;
            direction: rtl; /* للغة العربية */
        }

        a {
            text-decoration: none;
            color: var(--primary-color);
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        .container {
            max-width: 1200px;
            margin: auto;
            padding: 0 20px;
        }

        /* شريط التنقل (Navbar) */
        .navbar {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .navbar .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8em;
            font-weight: bold;
            color: var(--primary-color);
        }
        .logo span {
            color: var(--accent-color);
        }

        .nav-links {
            list-style: none;
            display: flex;
        }

        .nav-links li {
            margin-left: 30px;
        }

        .nav-links a {
            color: var(--text-color);
            font-weight: 500;
            transition: color 0.3s ease;
            display: flex;
            align-items: center;
        }
        .nav-links a:hover {
            color: var(--primary-color);
        }
        .nav-links a i {
            margin-left: 8px; /* مسافة بين الأيقونة والنص */
        }

        .cart-icon {
            position: relative;
            cursor: pointer;
        }
        .cart-icon i {
            font-size: 1.5em;
            color: var(--accent-color);
        }
        .cart-count {
            background-color: var(--secondary-color);
            color: var(--white);
            border-radius: 50%;
            padding: 3px 7px;
            font-size: 0.8em;
            position: absolute;
            top: -10px;
            right: -10px;
            animation: bounce 0.5s ease-out;
        }

        @keyframes bounce {
            0% { transform: scale(0.5); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }

        /* قسم الهيرو (الرئيسي) */
        .hero {
            background: linear-gradient(to right, #6dd5ed, #2193b0); /* تدرج أزرق منعش */
            color: var(--white);
            text-align: center;
            padding: 80px 20px;
            border-bottom-left-radius: 50px;
            border-bottom-right-radius: 50px;
            margin-bottom: 40px;
        }

        .hero h2 {
            font-size: 3em;
            margin-bottom: 15px;
            letter-spacing: 1px;
        }

        .hero p {
            font-size: 1.2em;
            margin-bottom: 30px;
            opacity: 0.9;
        }

        .btn {
            background-color: var(--secondary-color);
            color: var(--text-color);
            padding: 12px 25px;
            border-radius: 30px;
            font-weight: bold;
            transition: background-color 0.3s ease, transform 0.3s ease;
            display: inline-block;
        }

        .btn:hover {
            background-color: #FFD54F;
            transform: translateY(-3px);
        }
        .btn-primary {
            background-color: var(--primary-color);
            color: var(--white);
        }
        .btn-primary:hover {
            background-color: #5cb85c;
        }

        /* أقسام المنتجات */
        .section-title {
            text-align: center;
            font-size: 2.5em;
            color: var(--primary-color);
            margin-bottom: 40px;
            position: relative;
            padding-bottom: 10px;
        }
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--secondary-color);
            border-radius: 2px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }

        .product-card {
            background-color: var(--white);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            text-align: center;
        }
        .product-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.15);
        }

        .product-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-bottom: 1px solid #eee;
            transition: transform 0.3s ease;
        }
        .product-card:hover img {
            transform: scale(1.05);
        }

        .product-info {
            padding: 20px;
        }

        .product-info h3 {
            font-size: 1.4em;
            color: var(--accent-color);
            margin-bottom: 10px;
        }

        .product-info p.price {
            font-size: 1.6em;
            font-weight: bold;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .product-info .add-to-cart-btn {
            background-color: var(--primary-color);
            color: var(--white);
            padding: 10px 20px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1.1em;
            transition: background-color 0.3s ease;
            width: 100%;
        }
        .product-info .add-to-cart-btn:hover {
            background-color: #5cb85c;
        }
        .product-info .add-to-cart-btn i {
            margin-left: 8px;
        }

        /* سلة المشتريات (مودال - مخفية في البداية) */
        .cart-modal {
            display: none; /* مخفية افتراضياً */
            position: fixed;
            z-index: 1001;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.5); /* خلفية شبه شفافة */
            justify-content: center;
            align-items: center;
        }

        .cart-content {
            background-color: var(--white);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            width: 90%;
            max-width: 600px;
            position: relative;
            animation: slideInUp 0.5s ease-out;
        }
        @keyframes slideInUp {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .close-btn {
            color: var(--dark-gray);
            font-size: 2.2em;
            position: absolute;
            top: 15px;
            left: 20px;
            cursor: pointer;
            transition: color 0.3s ease;
        }
        .close-btn:hover {
            color: #d33;
        }

        .cart-content h2 {
            text-align: center;
            color: var(--primary-color);
            margin-bottom: 25px;
            font-size: 2em;
        }

        #cart-items {
            max-height: 300px;
            overflow-y: auto;
            margin-bottom: 20px;
            border-bottom: 1px solid #eee;
            padding-bottom: 15px;
        }

        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
            border-top: 1px solid #eee;
        }
        .cart-item:last-child {
            border-bottom: none;
        }

        .cart-item-info {
            display: flex;
            align-items: center;
        }
        .cart-item-info img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 8px;
            margin-left: 15px;
        }
        .cart-item-info span {
            font-weight: 600;
            color: var(--text-color);
            font-size: 1.1em;
        }

        .cart-item-actions {
            display: flex;
            align-items: center;
        }
        .cart-item-actions button {
            background-color: var(--light-bg);
            border: 1px solid #ddd;
            width: 30px;
            height: 30px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1em;
            color: var(--dark-gray);
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        .cart-item-actions button:hover {
            background-color: #e0e0e0;
            color: var(--text-color);
        }
        .cart-item-actions span {
            margin: 0 10px;
            font-weight: bold;
            font-size: 1.1em;
        }
        .remove-item-btn {
            background-color: #FFEBEE;
            color: #EF5350;
            border: 1px solid #EF5350;
            margin-right: 15px;
        }
        .remove-item-btn:hover {
            background-color: #EF5350;
            color: var(--white);
        }


        .cart-total {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 20px;
            font-size: 1.5em;
            font-weight: bold;
            color: var(--primary-color);
            padding-top: 15px;
            border-top: 2px dashed #eee;
        }

        .checkout-btn {
            width: 100%;
            padding: 15px;
            background-color: var(--primary-color);
            color: var(--white);
            border: none;
            border-radius: 30px;
            font-size: 1.3em;
            margin-top: 30px;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }
        .checkout-btn:hover {
            background-color: #5cb85c;
            transform: translateY(-3px);
        }
        .empty-cart-message {
            text-align: center;
            color: var(--dark-gray);
            font-style: italic;
            margin-top: 20px;
            font-size: 1.1em;
        }

        /* الفوتر (الختام) */
        .footer {
            background-color: var(--dark-gray);
            color: var(--white);
            text-align: center;
            padding: 30px 0;
            margin-top: 60px;
        }

        .footer p {
            margin: 0;
        }

        /* استجابة الشاشات الصغيرة */
        @media (max-width: 768px) {
            .navbar .container {
                flex-direction: column;
            }
            .nav-links {
                margin-top: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }
            .nav-links li {
                margin: 0 15px 10px;
            }
            .hero {
                padding: 60px 20px;
            }
            .hero h2 {
                font-size: 2.2em;
            }
            .section-title {
                font-size: 2em;
            }
        }

        @media (max-width: 480px) {
            .logo {
                font-size: 1.5em;
            }
            .nav-links {
                display: none; 
            }
            .hero h2 {
                font-size: 1.8em;
            }
            .hero p {
                font-size: 1em;
            }
            .product-grid {
                grid-template-columns: 1fr;
            }
        }

    </style>
</head>
<body>

    
<nav class="navbar">
        <div class="container">
            <a href="#" class="logo">سوبر ماركت <span>الحاضر</span></a>
            <ul class="nav-links">
                <li><a href="#products"><i class="fas fa-box"></i> المنتجات</a></li>
                <li><a href="#"><i class="fas fa-tags"></i> العروض</a></li>
                <li><a href="#"><i class="fas fa-info-circle"></i> عن المتجر</a></li>
                <li><a href="#"><i class="fas fa-phone-alt"></i> اتصل بنا</a></li>
            </ul>
            <div class="cart-icon" onclick="toggleCartModal()">
                <i class="fas fa-shopping-cart"></i>
                <span class="cart-count" id="cart-item-count">0</span>
            </div>
        </div>
    </nav>

    
<section class="hero">
        <div class="container">
            <h2>تسوق بذكاء، عش أسهل!</h2>
            <p>أفضل المنتجات الطازجة والأساسيات اليومية بأسعار لا تقبل المنافسة، توصيل سريع لباب بيتك.</p>
            <a href="#products" class="btn btn-primary">ابدأ التسوق الآن <i class="fas fa-arrow-left"></i></a>
        </div>
    </section>

    
<section id="products" class="products">
        <div class="container">
            <h2 class="section-title">منتجاتنا المميزة</h2>
            
            <div class="product-grid">
                
                <div class="product-card" data-id="p1" data-name="تفاح أحمر عضوي" data-price="12.50" data-img="https://images.pexels.com/photos/103130/pexels-photo-103130.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">
                    <img src="https://images.pexels.com/photos/103130/pexels-photo-103130.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="تفاح أحمر عضوي">
                    <div class="product-info">
                        <h3>تفاح أحمر عضوي</h3>
                        <p class="price">12.50 ر.س / كجم</p>
                        <button class="add-to-cart-btn" onclick="addToCart('p1', 'تفاح أحمر عضوي', 12.50, 'https://images.pexels.com/photos/103130/pexels-photo-103130.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')">
                            إضافة للسلة <i class="fas fa-cart-plus"></i>
                        </button>
                    </div>
                </div>

                <div class="product-card" data-id="p2" data-name="حليب طازج كامل الدسم" data-price="6.75" data-img="https://images.pexels.com/photos/1557022/pexels-photo-1557022.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">
                    <img src="https://images.pexels.com/photos/1557022/pexels-photo-1557022.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="حليب طازج كامل الدسم">
                    <div class="product-info">
                        <h3>حليب طازج كامل الدسم</h3>
                        <p class="price">6.75 ر.س / لتر</p>
                        <button class="add-to-cart-btn" onclick="addToCart('p2', 'حليب طازج كامل الدسم', 6.75, 'https://images.pexels.com/photos/1557022/pexels-photo-1557022.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')">
                            إضافة للسلة <i class="fas fa-cart-plus"></i>
                        </button>
                    </div>
                </div>

                <div class="product-card" data-id="p3" data-name="خبز أسمر يومي" data-price="3.00" data-img="https://images.pexels.com/photos/172287/pexels-photo-172287.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">
                    <img src="https://images.pexels.com/photos/172287/pexels-photo-172287.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="خبز أسمر يومي">
                    <div class="product-info">
                        <h3>خبز أسمر يومي</h3>
                        <p class="price">3.00 ر.س / عبوة</p>
                        <button class="add-to-cart-btn" onclick="addToCart('p3', 'خبز أسمر يومي', 3.00, 'https://images.pexels.com/photos/172287/pexels-photo-172287.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')">
                            إضافة للسلة <i class="fas fa-cart-plus"></i>
                        </button>
                    </div>
                </div>

                <div class="product-card" data-id="p4" data-name="بيض بلدي طازج" data-price="15.99" data-img="https://images.pexels.com/photos/162712/pexels-photo-162712.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">
                    <img src="https://images.pexels.com/photos/162712/pexels-photo-162712.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="بيض بلدي طازج">
                    <div class="product-info">
                        <h3>بيض بلدي طازج</h3>
                        <p class="price">15.99 ر.س / طبق</p>
                        <button class="add-to-cart-btn" onclick="addToCart('p4', 'بيض بلدي طازج', 15.99, 'https://images.pexels.com/photos/162712/pexels-photo-162712.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')">
                            إضافة للسلة <i class="fas fa-cart-plus"></i>
                        </button>
                    </div>
                </div>

                <div class="product-card" data-id="p5" data-name="مياه معدنية (6 عبوات)" data-price="8.00" data-img="https://images.pexels.com/photos/208573/pexels-photo-208573.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">
                    <img src="https://images.pexels.com/photos/208573/pexels-photo-208573.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="مياه معدنية (6 عبوات)">
                    <div class="product-info">
                        <h3>مياه معدنية (6 عبوات)</h3>
                        <p class="price">8.00 ر.س</p>
                        <button class="add-to-cart-btn" onclick="addToCart('p5', 'مياه معدنية (6 عبوات)', 8.00, 'https://images.pexels.com/photos/208573/pexels-photo-208573.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')">
                            إضافة للسلة <i class="fas fa-cart-plus"></i>
                        </button>
                    </div>
                </div>

                <div class="product-card" data-id="p6" data-name="زيت زيتون بكر ممتاز" data-price="35.50" data-img="https://images.pexels.com/photos/1230623/pexels-photo-1230623.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1">
                    <img src="https://images.pexels.com/photos/1230623/pexels-photo-1230623.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="زيت زيتون بكر ممتاز">
                    <div class="product-info">
                        <h3>زيت زيتون بكر ممتاز</h3>
                        <p class="price">35.50 ر.س / 750 مل</p>
                        <button class="add-to-cart-btn" onclick="addToCart('p6', 'زيت زيتون بكر ممتاز', 35.50, 'https://images.pexels.com/photos/1230623/pexels-photo-1230623.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')">
                            إضافة للسلة <i class="fas fa-cart-plus"></i>
                        </button>
                    </div>
                </div>
                
            </div>
        </div>
    </section>

    
<div id="cartModal" class="cart-modal">
        <div class="cart-content">
            <span class="close-btn" onclick="toggleCartModal()">&times;</span>
            <h2>سلة المشتريات <i class="fas fa-shopping-basket"></i></h2>
            <div id="cart-items">
                
<p class="empty-cart-message" id="empty-cart-msg">سلتك فارغة حاليًا!</p>
            </div>
            <div class="cart-total">
                <span>الإجمالي:</span>
                <span id="cart-total-price">0.00 ر.س</span>
            </div>
            <button class="checkout-btn" onclick="checkout()">إتمام الطلب <i class="fas fa-credit-card"></i></button>
        </div>
    </div>

    
<footer class="footer">
        <div class="container">
            <p>&copy; 2024 سوبر ماركت الحاضر. جميع الحقوق محفوظة.</p>
            <p>صمم بواسطة <a href="#" style="color: var(--secondary-color);">فريق الحاضر</a></p>
        </div>
    </footer>

    
<script>
        let cart = []; // مصفوفة لتخزين المنتجات في السلة

        // دالة لفتح/إغلاق سلة المشتريات
        function toggleCartModal() {
            const cartModal = document.getElementById('cartModal');
            if (cartModal.style.display === 'flex') {
                cartModal.style.display = 'none';
            } else {
                cartModal.style.display = 'flex';
                renderCart(); // عرض محتويات السلة عند الفتح
            }
        }

        // دالة لإضافة منتج إلى السلة
        function addToCart(id, name, price, img) {
            const existingItem = cart.find(item => item.id === id);
            if (existingItem) {
                existingItem.quantity++;
            } else {
                cart.push({ id, name, price, img, quantity: 1 });
            }
            updateCartCount();
            // يمكنك استخدام alert أو نظام إشعارات أفضل هنا
        }

        // دالة لتحديث عدد المنتجات في أيقونة السلة
        function updateCartCount() {
            const count = cart.reduce((total, item) => total + item.quantity, 0);
            document.getElementById('cart-item-count').textContent = count;
        }

        // دالة لعرض المنتجات داخل المودال (سلة المشتريات)
        function renderCart() {
            const cartItemsContainer = document.getElementById('cart-items');
            const cartTotalPrice = document.getElementById('cart-total-price');
            const emptyCartMsg = document.getElementById('empty-cart-msg');
            let total = 0;
            cartItemsContainer.innerHTML = ''; // تفريغ المحتوى الحالي

            if (cart.length === 0) {
                emptyCartMsg.style.display = 'block';
            } else {
                emptyCartMsg.style.display = 'none';
                cart.forEach(item => {
                    const itemElement = document.createElement('div');
                    itemElement.classList.add('cart-item');
                    itemElement.innerHTML = `
                        <div class="cart-item-info">
                            <img src="${item.img}" alt="${item.name}">
                            <span>${item.name}</span>
                        </div>
                        <div class="cart-item-actions">
                            <button onclick="changeQuantity('${item.id}', -1)">-</button>
                            <span>${item.quantity}</span>
                            <button onclick="changeQuantity('${item.id}', 1)">+</button>
                            <span style="margin-right: 15px; font-weight: normal;">${(item.price * item.quantity).toFixed(2)} ر.س</span>
                            <button class="remove-item-btn" onclick="removeItem('${item.id}')"><i class="fas fa-trash-alt"></i></button>
                        </div>
                    `;
                    cartItemsContainer.appendChild(itemElement);
                    total += item.price * item.quantity;
                });
            }

            cartTotalPrice.textContent = `${total.toFixed(2)} ر.س`;
        }

        // دالة لتغيير كمية منتج في السلة
        function changeQuantity(id, change) {
            const item = cart.find(item => item.id === id);
            if (item) {
                item.quantity += change;
                if (item.quantity <= 0) {
                    removeItem(id); // إزالة المنتج إذا أصبحت الكمية صفر أو أقل
                }
            }
            updateCartCount();
            renderCart();
        }

        // دالة لإزالة منتج من السلة
        function removeItem(id) {
            cart = cart.filter(item => item.id !== id);
            updateCartCount();
            renderCart();
        }

        // دالة إتمام الطلب (هنا مجرد رسالة تنبيه)
        function checkout() {
            if (cart.length === 0) {
                alert('سلتك فارغة. الرجاء إضافة بعض المنتجات قبل إتمام الطلب.');
                return;
            }
            const total = cart.reduce((sum, item) => sum + item.price * item.quantity, 0);
            alert(`جاري إتمام طلبك بقيمة: ${total.toFixed(2)} ر.س.\nشكراً لتسوقك من سوبر ماركت الحاضر!`);
            cart = []; // تفريغ السلة بعد إتمام الطلب
            updateCartCount();
            renderCart();
            toggleCartModal(); // إغلاق السلة
        }

        // تحديث عدد السلة عند تحميل الصفحة 
        document.addEventListener('DOMContentLoaded', updateCartCount);

    </script>
</body>
</html>
