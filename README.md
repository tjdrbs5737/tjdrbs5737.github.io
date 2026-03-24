<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>프리미엄 헤비웨이트 스웨트 팬츠</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;400;700;900&display=swap');
        body { font-family: 'Noto Sans KR', sans-serif; }
        .sticky-nav { position: sticky; top: 0; background: white; z-index: 50; border-bottom: 1px solid #eee; }
    </style>
</head>
<body class="text-gray-900 leading-tight">

    <main class="max-w-6xl mx-auto px-4 py-8 md:py-16">
        <div class="flex flex-col md:flex-row gap-12">
            
            <div class="w-full md:w-[55%] space-y-4">
                <img src="https://images.unsplash.com/photo-1552066344-2464c9732689?auto=format&fit=crop&q=80&w=1000" 
                     class="w-full rounded-xl shadow-lg" alt="상품 메인">
                <div class="grid grid-cols-2 gap-4">
                    <img src="https://images.unsplash.com/photo-1605518216938-7c31b7b14ad0?auto=format&fit=crop&q=80&w=500" class="rounded-lg">
                    <img src="https://images.unsplash.com/photo-1594633312681-425c7b97ccd1?auto=format&fit=crop&q=80&w=500" class="rounded-lg">
                </div>
            </div>

            <div class="w-full md:w-[45%] flex flex-col justify-start">
                <div class="mb-6">
                    <span class="inline-block bg-black text-white text-[10px] px-2 py-1 mb-3">BEST SELLER</span>
                    <h1 class="text-3xl font-black mb-2 tracking-tighter text-slate-900">헤비웨이트 와이드 테리 스웨트 팬츠</h1>
                    <p class="text-gray-500 text-sm">탄탄한 고중량 원단으로 완성한 압도적 실루엣</p>
                </div>

                <div class="flex items-center gap-4 mb-8">
                    <span class="text-3xl font-bold text-blue-600 tracking-tighter">30%</span>
                    <span class="text-3xl font-bold tracking-tighter">34,300원</span>
                    <span class="text-xl text-gray-300 line-through">49,000원</span>
                </div>

                <div class="space-y-6 border-t border-gray-100 pt-8">
                    <div>
                        <label class="block text-xs font-bold text-gray-400 mb-3 uppercase tracking-widest">Select Color</label>
                        <div class="flex gap-3">
                            <button class="w-10 h-10 rounded-full bg-gray-400 border-2 border-black ring-2 ring-offset-2 ring-black"></button>
                            <button class="w-10 h-10 rounded-full bg-black"></button>
                            <button class="w-10 h-10 rounded-full bg-stone-200"></button>
                        </div>
                    </div>

                    <div>
                        <label class="block text-xs font-bold text-gray-400 mb-3 uppercase tracking-widest">Select Size</label>
                        <div class="grid grid-cols-3 gap-2 text-sm font-bold">
                            <button class="border py-4 hover:bg-black hover:text-white transition rounded">M</button>
                            <button class="border py-4 hover:bg-black hover:text-white transition rounded">L</button>
                            <button class="border py-4 bg-gray-50 text-gray-300 cursor-not-allowed rounded" disabled>XL (품절)</button>
                        </div>
                    </div>
                </div>

                <div class="mt-10 flex flex-col gap-3">
                    <button class="w-full bg-black text-white py-5 font-black text-lg hover:bg-gray-800 transition rounded-lg">
                        BUY NOW (바로 구매)
                    </button>
                    <div class="flex gap-3">
                        <button class="flex-1 border border-gray-200 py-4 font-bold text-gray-700 hover:bg-gray-50 transition rounded-lg">장바구니</button>
                        <button class="flex-1 border border-gray-200 py-4 font-bold text-gray-700 hover:bg-gray-50 transition rounded-lg">위시리스트</button>
                    </div>
                </div>

                <p class="text-xs text-center text-gray-400 mt-6 font-medium">전 지역 무료 배송 · 7일 이내 자유로운 반품 가능</p>
            </div>
        </div>
    </main>

    <nav class="sticky-nav">
        <div class="max-w-4xl mx-auto flex text-sm font-bold">
            <a href="#content" class="flex-1 py-5 text-center border-b-2 border-black text-black">DETAIL</a>
            <a href="#guide" class="flex-1 py-5 text-center text-gray-400">GUIDE</a>
            <a href="#review" class="flex-1 py-5 text-center text-gray-400">REVIEWS</a>
        </div>
    </nav>

    <article id="content" class="max-w-4xl mx-auto py-20 px-4 space-y-24">
        
        <div class="text-center space-y-6">
            <h2 class="text-sm font-bold tracking-[0.3em] text-blue-600">01. FABRIC</h2>
            <p class="text-5xl font-black tracking-tighter">무게감이 만드는<br>압도적 실루엣</p>
            <p class="text-gray-500 max-w-lg mx-auto leading-relaxed">평범한 쭈리 원단이 아닙니다. 야드당 950g의 고중량 원단으로 제작되어, 세탁 후에도 형태가 무너지지 않고 묵직하게 떨어지는 핏을 선사합니다.</p>
            <img src="https://images.unsplash.com/photo-1620799140408-edc6dcb6d633?auto=format&fit=crop&q=80&w=1200" class="w-full rounded-3xl mt-10">
        </div>

        <div class="grid md:grid-cols-2 gap-10 items-center bg-gray-50 p-10 rounded-[3rem]">
            <img src="https://images.unsplash.com/photo-1591195853828-11db59a44f6b?auto=format&fit=crop&q=80&w=600" class="rounded-2xl shadow-xl">
            <div class="space-y-4">
                <h2 class="text-sm font-bold tracking-[0.3em] text-blue-600">02. SEWING</h2>
                <h3 class="text-3xl font-black italic">"CRAFTMANSHIP"</h3>
                <p class="text-gray-500 leading-relaxed font-medium">프리미엄 브랜드에서만 사용하는 갈라삼봉 공법을 적용했습니다. 허리 밴드부터 밑단까지 이질감 없는 부드러운 착용감을 보장합니다.</p>
            </div>
        </div>

        <div class="space-y-4">
            <img src="https://images.unsplash.com/photo-1552066344-2464c9732689?auto=format&fit=crop&q=80&w=1200" class="w-full rounded-2xl">
            <p class="text-center text-gray-400 text-sm italic">Model: 184cm / 72kg (Wearing L size)</p>
        </div>

    </article>

    <footer class="bg-black text-white py-20 px-4 text-center">
        <p class="text-2xl font-black tracking-tighter mb-4">G-M-N BRAND SHOP</p>
        <p class="text-gray-500 text-xs">Copyright © 2026. All Rights Reserved.</p>
    </footer>

</body>
</html>
