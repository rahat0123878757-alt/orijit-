<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>অরিজিৎ দুধওয়ালা | অনলাইন দুধ অর্ডার করুন</title>
    <!-- Tailwind CSS লোড করা হচ্ছে -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* ইন্টার ফন্ট ব্যবহার করা হচ্ছে */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #ffffff; /* প্রধান থিম: সাদা */
            color: #1f2937;
        }
        .header-bg {
            background-color: #f3f4f6; /* হালকা ধূসর (হেডার বা ফুটারের জন্য) */
        }
        .primary-color {
            color: #1e40af; /* ডিপ নীল */
        }
        .bg-primary {
            background-color: #1e40af;
        }
        .hover-primary:hover {
            background-color: #3b82f6;
        }
        .milk-product-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .milk-product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(30, 64, 175, 0.1), 0 4px 6px -2px rgba(30, 64, 175, 0.05);
        }
        .gallery-image {
            width: 100%;
            height: 250px; /* নির্দিষ্ট উচ্চতা */
            object-fit: cover;
            transition: transform 0.3s ease;
        }
        .gallery-image:hover {
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    
    <!-- নেভিগেশন বার -->
    <nav class="header-bg shadow-md sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- ব্র্যান্ড নাম -->
                <a href="#" class="text-2xl font-extrabold primary-color tracking-wide">
                    অরিজিৎ দুধওয়ালা
                </a>

                <!-- মেনু আইটেম -->
                <div class="flex space-x-4 text-sm font-semibold">
                    <a href="#products" class="text-gray-600 hover:text-blue-600 transition duration-200 hidden sm:inline">পণ্য</a>
                    <a href="#gallery" class="text-gray-600 hover:text-blue-600 transition duration-200 hidden sm:inline">গ্যালারি</a>
                    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition duration-200 hidden sm:inline">যোগাযোগ</a>
                    <a href="#order" class="bg-blue-600 text-white px-3 py-1 rounded-lg hover:bg-blue-700 transition duration-200 shadow-md">অর্ডার করুন</a>
                </div>
                <!-- মোবাইল মেনুর জন্য একটি হ্যামবার্গার আইকন যোগ করা যেতে পারে, তবে সরলতার জন্য এখানে বাদ দেওয়া হলো -->
            </div>
        </div>
    </nav>
    
    <!-- প্রধান কন্টেইনার -->
    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10">

        <!-- বিক্রেতার তথ্য (Seller Info) -->
        <section id="seller-info" class="mb-16 text-center bg-blue-50 p-10 rounded-xl shadow-lg border-t-4 border-blue-500">
            <h1 class="text-4xl sm:text-5xl font-extrabold primary-color mb-3">বিশুদ্ধ দুধের বিশ্বস্ত নাম</h1>
            <p class="text-xl text-gray-600 mb-6">সরাসরি খামার থেকে আপনার দরজায় সেরা পণ্য</p>

            <div class="flex flex-col items-center justify-center space-y-4">
                <!-- বিক্রেতা অরিজিৎ এর ছবি -->
                <img src="https://i.postimg.cc/P5QF6hGR/Screenshot-20251108-153605.jpg" alt="বিক্রেতা অরিজিৎ এর ছবি" class="w-32 h-32 object-cover rounded-full border-4 border-white shadow-xl bg-gray-200" onerror="this.onerror=null;this.src='https://placehold.co/150x150/ffffff/1e40af?text=Orijit'">
                
                <div class="text-center">
                    <h2 class="text-2xl font-bold text-gray-800">অরিজিৎ (Orijit)</h2>
                    <p class="text-lg text-gray-500">দুধ বিক্রেতা ও স্বত্বাধিকারী</p>
                </div>
            </div>
        </section>

        <!-- পণ্যের তালিকা (Product List) -->
        <section id="products" class="mb-16">
            <h2 class="text-3xl font-bold primary-color mb-8 border-b-2 border-blue-300 pb-3">আমাদের বিশুদ্ধ পণ্যসমূহ</h2>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- পণ্য ১: গরুর দুধ -->
                <div class="milk-product-card bg-white p-6 rounded-xl shadow-lg border border-gray-100">
                    <div class="text-4xl mb-4 text-center">🥛</div>
                    <h3 class="text-xl font-bold primary-color mb-2">ফুল ক্রিম গরুর দুধ</h3>
                    <p class="text-gray-600 mb-3">সরাসরি খামার থেকে সংগৃহীত, কোনো মেশানো নেই। ১০০% খাঁটি।</p>
                    <p class="text-2xl font-extrabold text-green-600">৳ ৬০ / লিটার</p>
                    <button onclick="document.getElementById('product_milk').value = 'ফুল ক্রিম গরুর দুধ (৳ ৬০/লিটার)'; document.getElementById('order').scrollIntoView({ behavior: 'smooth' });" class="mt-4 w-full bg-blue-500 text-white py-2 rounded-lg hover-primary transition duration-200 shadow-md">অর্ডার করতে যোগ করুন</button>
                </div>

                <!-- পণ্য ২: দই -->
                <div class="milk-product-card bg-white p-6 rounded-xl shadow-lg border border-gray-100">
                    <div class="text-4xl mb-4 text-center">🍚</div>
                    <h3 class="text-xl font-bold primary-color mb-2">ঘরে পাতা মিষ্টি দই</h3>
                    <p class="text-gray-600 mb-3">ঐতিহ্যবাহী পদ্ধতিতে তৈরি সুস্বাদু মিষ্টি দই। উৎসবের জন্য সেরা।</p>
                    <p class="text-2xl font-extrabold text-green-600">৳ ১৪০ / ৫০০ গ্রাম</p>
                    <button onclick="document.getElementById('product_milk').value = 'মিষ্টি দই (৳ ১৪০/ ৫০০ গ্রাম)'; document.getElementById('order').scrollIntoView({ behavior: 'smooth' });" class="mt-4 w-full bg-blue-500 text-white py-2 rounded-lg hover-primary transition duration-200 shadow-md">অর্ডার করতে যোগ করুন</button>
                </div>

                <!-- পণ্য ৩: ঘি -->
                <div class="milk-product-card bg-white p-6 rounded-xl shadow-lg border border-gray-100">
                    <div class="text-4xl mb-4 text-center">🧈</div>
                    <h3 class="text-xl font-bold primary-color mb-2">খাঁটি দেশি ঘি</h3>
                    <p class="text-gray-600 mb-3">হাতের তৈরি সুগন্ধযুক্ত ঘি, যা খাবারের স্বাদ বাড়িয়ে দেবে।</p>
                    <p class="text-2xl font-extrabold text-green-600">৳ ৪৫০ / ২৫০ গ্রাম</p>
                    <button onclick="document.getElementById('product_milk').value = 'খাঁটি দেশি ঘি (৳ ৪৫০/২৫০ গ্রাম)'; document.getElementById('order').scrollIntoView({ behavior: 'smooth' });" class="mt-4 w-full bg-blue-500 text-white py-2 rounded-lg hover-primary transition duration-200 shadow-md">অর্ডার করতে যোগ করুন</button>
                </div>
            </div>
        </section>

        <!-- গ্যালারি সেকশন (Gallery Section) -->
        <section id="gallery" class="mb-16">
            <h2 class="text-3xl font-bold primary-color mb-8 border-b-2 border-blue-300 pb-3">আমাদের খামার ও গ্যালারি</h2>

            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                
                <!-- গ্যালারি আইটেম ১: দুধ সরবরাহ -->
                <div class="overflow-hidden rounded-lg shadow-md">
                    <img src="(https://i.postimg.cc/DyjvgFz2/Gemini-Generated-Image-tkuaertkuaertkua.png=Milk+Delivery" alt="দুধ সরবরাহ" class="gallery-image">
                    <p class="text-center text-sm p-2 text-gray-600 bg-gray-50">সকালের তাজা দুধ</p>
                </div>

                <!-- গ্যালারি আইটেম ২: খামারের দৃশ্য -->
                <div class="overflow-hidden rounded-lg shadow-md">
                    <img src="https://placehold.co/600x400/10b981/ffffff?text=Farm+View" alt="খামারের দৃশ্য" class="gallery-image">
                    <p class="text-center text-sm p-2 text-gray-600 bg-gray-50">স্বাস্থ্যকর পরিবেশ</p>
                </div>

                <!-- গ্যালারি আইটেম ৩: দই তৈরি -->
                <div class="overflow-hidden rounded-lg shadow-md">
                    <img src="https://placehold.co/600x400/ef4444/ffffff?text=Yogurt+Making" alt="দই তৈরি" class="gallery-image">
                    <p class="text-center text-sm p-2 text-gray-600 bg-gray-50">ঐতিহ্যবাহী দই</p>
                </div>

                <!-- গ্যালারি আইটেম ৪: অরিজিৎ ভাই -->
                <div class="overflow-hidden rounded-lg shadow-md">
                    <img src="https://placehold.co/600x400/f59e0b/ffffff?text=Orijit+Dudhwala" alt="অরিজিৎ দুধওয়ালা" class="gallery-image">
                    <p class="text-center text-sm p-2 text-gray-600 bg-gray-50">আমাদের বিক্রেতা</p>
                </div>
            </div>
            <p class="text-center text-sm text-gray-500 mt-6">গ্যালারির ছবিগুলো পরিবর্তন করতে ছবির লিংকগুলো বদলে দিন।</p>
        </section>

        <!-- যোগাযোগ সেকশন (Contact Section) -->
        <section id="contact" class="mb-16 bg-white p-8 rounded-xl shadow-2xl border-t-4 border-red-500">
            <h2 class="text-3xl font-bold primary-color mb-6 border-b-2 border-red-300 pb-3">যোগাযোগ করুন</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-lg">
                <div>
                    <h3 class="font-bold text-gray-800 mb-3">যোগাযোগের তথ্য:</h3>
                    <p class="text-gray-600 mb-2">📞 ফোন: 018XXXXXXXX (অরিজিৎ)</p>
                    <p class="text-gray-600 mb-2">✉️ ইমেল: orijitdudhwala@example.com</p>
                    <p class="text-gray-600 mb-2">📍 ঠিকানা: ঢাকা, বাংলাদেশ (ডেমো ঠিকানা)</p>
                </div>

                <div>
                    <h3 class="font-bold text-gray-800 mb-3">আমরা ম্যাপে:</h3>
                    <!-- Google Maps এম্বেড প্লেসহোল্ডার -->
                    <iframe 
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d116837.26085189736!2d90.33230491008775!3d23.78082607831006!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755b8b087029b47%3A0x88f09d8fcd671e88!2sDhaka!5e0!3m2!1sen!2sbd!4v1700000000000!5m2!1sen!2sbd" 
                        width="100%" 
                        height="200" 
                        style="border:0;" 
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade"
                        class="rounded-lg shadow-md"
                    ></iframe>
                </div>
            </div>
        </section>


        <!-- অনলাইন অর্ডারিং সিস্টেম (Online Order System) -->
        <section id="order" class="mb-16 bg-white p-8 rounded-xl shadow-2xl border-t-4 border-green-500">
            <h2 class="text-3xl font-bold primary-color mb-6 border-b-2 border-green-300 pb-3">অনলাইন অর্ডারের জন্য ফর্ম</h2>
            <p class="text-gray-600 mb-6">নিচের ফর্মটি পূরণ করে অর্ডার নিশ্চিত করুন। অর্ডার সফল হলে অরিজিৎ ভাই দ্রুত আপনার সাথে যোগাযোগ করবেন।</p>
            
            <form id="orderForm" class="space-y-4">
                
                <!-- নির্বাচিত পণ্য -->
                <div>
                    <label for="product_milk" class="block text-gray-700 font-semibold mb-2">আপনি কি অর্ডার করতে চান?</label>
                    <input type="text" id="product_milk" name="product_milk" value="ফুল ক্রিম গরুর দুধ (৳ ৬০/লিটার)" required class="w-full p-3 border border-gray-300 rounded-lg bg-gray-50 focus:border-blue-500">
                </div>

                <!-- পরিমাণ -->
                <div>
                    <label for="quantity" class="block text-gray-700 font-semibold mb-2">পরিমাণ (লিটার/গ্রাম/পিস)</label>
                    <input type="number" id="quantity" name="quantity" min="1" value="1" required class="w-full p-3 border border-gray-300 rounded-lg focus:border-blue-500">
                </div>

                <!-- গ্রাহকের নাম -->
                <div>
                    <label for="customer_name" class="block text-gray-700 font-semibold mb-2">আপনার পুরো নাম</label>
                    <input type="text" id="customer_name" name="customer_name" required class="w-full p-3 border border-gray-300 rounded-lg focus:border-blue-500">
                </div>

                <!-- ফোন নম্বর -->
                <div>
                    <label for="phone" class="block text-gray-700 font-semibold mb-2">ফোন নম্বর (যোগাযোগের জন্য)</label>
                    <input type="tel" id="phone" name="phone" pattern="[0-9]{11}" placeholder="উদাহরণ: ০১৭xxxxxxxx" required class="w-full p-3 border border-gray-300 rounded-lg focus:border-blue-500">
                </div>

                <!-- ঠিকানা -->
                <div>
                    <label for="address" class="block text-gray-700 font-semibold mb-2">ডেলিভারির ঠিকানা</label>
                    <textarea id="address" name="address" rows="3" required class="w-full p-3 border border-gray-300 rounded-lg focus:border-blue-500"></textarea>
                </div>
                
                <!-- পেমেন্ট মেথড -->
                <div>
                    <label class="block text-gray-700 font-semibold mb-2">পেমেন্ট পদ্ধতি</label>
                    <div class="flex space-x-4">
                        <label class="flex items-center">
                            <input type="radio" name="payment" value="Cash on Delivery" checked class="form-radio text-blue-600">
                            <span class="ml-2 text-gray-700">ক্যাশ অন ডেলিভারি</span>
                        </label>
                        <label class="flex items-center">
                            <input type="radio" name="payment" value="Online Payment" class="form-radio text-blue-600">
                            <span class="ml-2 text-gray-700">অনলাইন পেমেন্ট (বিকাশ/নগদ)</span>
                        </label>
                    </div>
                </div>

                <div id="messageBox" class="text-center text-red-600 font-semibold mt-4 hidden"></div>

                <button type="submit" class="w-full bg-green-600 text-white py-3 rounded-lg hover:bg-green-700 transition duration-200 font-bold text-lg shadow-xl">
                    অর্ডার নিশ্চিত করুন (Confirm Order)
                </button>
            </form>
        </section>


        <!-- ফুটার -->
        <footer class="mt-12 p-6 text-center text-gray-500 border-t border-gray-200">
            <p class="text-sm">&copy; ২০২৫ অরিজিৎ দুধওয়ালা। সমস্ত অধিকার সংরক্ষিত।</p>
            <p class="text-xs mt-2">Design & Development: Developed by **rm71 team** & **Rahat** (owner of rm71 team)</p>
        </footer>

    </main>

    <!-- JavaScript For Order Submission & Messaging -->
    <script>
        const messageBox = document.getElementById('messageBox');
        const orderForm = document.getElementById('orderForm');

        // কাস্টম মেসেজ দেখানোর ফাংশন (alert() এর বিকল্প)
        function showMessage(message, isSuccess = true) {
            messageBox.textContent = message;
            messageBox.className = `text-center font-semibold mt-4 p-3 rounded-lg shadow-md ${isSuccess ? 'bg-green-100 text-green-700' : 'bg-red-100 text-red-700'}`;
            messageBox.style.display = 'block';
            
            // 5 সেকেন্ড পর মেসেজ হাইড করে দেবে
            setTimeout(() => {
                messageBox.style.display = 'none';
            }, 5000);
        }

        orderForm.addEventListener('submit', function(e) {
            e.preventDefault();

            // এখানে Firestore ডাটাবেস না থাকায়, আমরা শুধু একটি সাকসেস মেসেজ দেখাবো।
            
            const formData = new FormData(orderForm);
            const data = {};
            formData.forEach((value, key) => {
                data[key] = value;
            });

            console.log("অর্ডার ডেটা:", data);

            // সফল মেসেজ
            showMessage(`আপনার অর্ডার সফলভাবে নিশ্চিত করা হয়েছে! (${data.product_milk}, পরিমাণ: ${data.quantity})। অরিজিৎ ভাই দ্রুত আপনার সাথে যোগাযোগ করবেন।`, true);

            // ফর্মটি রিসেট করুন
            orderForm.reset();
            // ডিফল্ট ভ্যালু সেট করুন
            document.getElementById('product_milk').value = document.querySelector('.milk-product-card h3').textContent.trim() + ' (' + document.querySelector('.milk-product-card p:last-of-type').textContent.trim() + ')'; 
        });

    </script>
</body>
</html>
