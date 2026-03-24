import React, { useState, useEffect } from 'react';

// 공통 컴포넌트: 섹션 제목
const SectionTitle = ({ title, sub }) => (
  <div className="text-center my-20">
    <h3 className="text-3xl font-black tracking-tight mb-2 uppercase">{title}</h3>
    <p className="text-gray-400 text-sm">{sub}</p>
  </div>
);

const ProductDetail = ({ testGroup }) => {
  return (
    <div className="bg-white min-h-screen font-sans text-gray-900">
      {/* 1. 네비게이션 */}
      <nav className="sticky top-0 z-[60] bg-white border-b px-6 py-4 flex justify-between items-center">
        <h1 className="font-black text-2xl tracking-tighter cursor-pointer">MUSINSA STANDARD</h1>
        <div className="hidden md:flex space-x-6 text-xs font-bold uppercase tracking-widest">
          <span>Men</span><span>Women</span><span>Kids</span><span>Beauty</span>
        </div>
      </nav>

      <main className="max-w-7xl mx-auto flex flex-col md:flex-row px-4 pt-10 gap-12">
        
        {/* 왼쪽: 아주 긴 상세 이미지 영역 */}
        <div className="w-full md:w-[65%]">
          {/* 메인 이미지 */}
          <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_5_500.jpg" alt="Main" className="w-full mb-10 shadow-sm" />

          {/* 특징 섹션 */}
          <SectionTitle title="Product Features" sub="최적의 핏을 위한 무신사만의 디테일" />
          <div className="space-y-4">
            <div className="bg-gray-50 p-10 rounded-xl text-center">
              <p className="text-lg font-medium leading-relaxed">
                "사계절 내내 입기 좋은 적당한 두께감과<br/>
                신축성이 뛰어난 T/R 소재를 사용하여 편안한 착용감을 선사합니다."
              </p>
            </div>
            <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_1_500.jpg" className="w-full h-[800px] object-cover" alt="Detail 1" />
          </div>

          {/* 모델 착용샷 (길게 나열) */}
          <SectionTitle title="Editorial Look" sub="186cm / 72kg - 32 Size Wearing" />
          <div className="grid grid-cols-1 gap-6">
            <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_2_500.jpg" className="w-full h-[1000px] object-cover" alt="Model 1" />
            <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_3_500.jpg" className="w-full h-[1000px] object-cover" alt="Model 2" />
          </div>

          {/* 디테일 컷 */}
          <SectionTitle title="Close Up" sub="마감 하나까지 신경 쓴 프리미엄 퀄리티" />
          <div className="grid grid-cols-2 gap-4">
            <div className="h-96 bg-gray-200 flex items-center justify-center font-bold">허리 밴딩 디테일</div>
            <div className="h-96 bg-gray-200 flex items-center justify-center font-bold">YKK 지퍼 사용</div>
            <div className="h-96 bg-gray-200 flex items-center justify-center font-bold">밑단 마감 처리</div>
            <div className="h-96 bg-gray-200 flex items-center justify-center font-bold">백 포켓 디자인</div>
          </div>

          {/* 사이즈 가이드 */}
          <SectionTitle title="Size Guide" sub="실측 사이즈를 확인하세요" />
          <table className="w-full border-t border-b border-black text-sm text-center mb-40">
            <thead className="bg-gray-50 font-bold">
              <tr>
                <th className="py-4 border-b">Size (cm)</th>
                <th className="py-4 border-b">총장</th>
                <th className="py-4 border-b">허리단면</th>
                <th className="py-4 border-b">허벅지단면</th>
              </tr>
            </thead>
            <tbody>
              <tr><td className="py-4 border-b">28</td><td className="py-4 border-b">102</td><td className="py-4 border-b">37.5</td><td className="py-4 border-b">31.5</td></tr>
              <tr><td className="py-4 border-b font-bold text-blue-600">30 (Best)</td><td className="py-4 border-b">103</td><td className="py-4 border-b">40</td><td className="py-4 border-b">32.7</td></tr>
              <tr><td className="py-4 border-b">32</td><td className="py-4 border-b">104</td><td className="py-4 border-b">42.5</td><td className="py-4 border-b">33.9</td></tr>
            </tbody>
          </table>
        </div>

        {/* 오른쪽: 상품 정보 및 결제창 (Sticky) */}
        <div className="w-full md:w-[35%] relative">
          <div className="sticky top-28 space-y-8">
            <div className="pb-6 border-b-2 border-black">
              <h2 className="text-3xl font-black leading-tight mb-2">릴렉스드 와이드 슬랙스 [블랙]</h2>
              <div className="flex items-center space-x-3 mt-4">
                <span className="bg-red-500 text-white px-2 py-1 text-xs font-bold">-10%</span>
                <span className="text-2xl font-black">32,900원</span>
                <span className="text-gray-400 line-through text-lg italic">36,900원</span>
              </div>
            </div>

            <div className="space-y-4 text-sm font-medium">
              <div className="flex justify-between"><span>브랜드/품번</span><span className="underline font-bold text-blue-700">MUSINSA STANDARD / MSS-1844582</span></div>
              <div className="flex justify-between"><span>누적판매</span><span>1.2만개+</span></div>
              <div className="flex justify-between"><span>구매후기</span><span className="text-yellow-500">★★★★★ (4,821)</span></div>
            </div>

            {/* A안: 최상단 구매 버튼 영역 (스크롤해도 여기 그대로 있음) */}
            {testGroup === 'A' && (
              <div className="flex flex-col gap-3 py-6 border-y bg-white">
                <button className="w-full bg-black text-white py-5 font-black text-lg hover:bg-zinc-800 active:scale-95 transition">바로 구매하기</button>
                <div className="flex gap-2">
                  <button className="flex-1 border border-zinc-300 py-4 font-bold hover:bg-zinc-50 transition uppercase">Cart</button>
                  <button className="flex-1 border border-zinc-300 py-4 font-bold hover:bg-zinc-50 transition uppercase">Wish</button>
                </div>
              </div>
            )}

            <div className="bg-zinc-50 p-5 rounded-lg text-xs leading-relaxed text-gray-500">
              <p>• 멤버십 등급별 추가 할인이 적용됩니다.</p>
              <p>• 첫 구매 시 10,000원 할인 쿠폰 증정</p>
            </div>
          </div>
        </div>
      </main>

      {/* B안: 따라다니는 플로팅 구매 바 (전체 너비) */}
      {testGroup === 'B' && (
        <div className="fixed bottom-0 left-0 w-full bg-white border-t border-zinc-200 p-4 z-[100] shadow-[0_-10px_30px_rgba(0,0,0,0.08)] animate-in slide-in-from-bottom duration-500">
          <div className="max-w-7xl mx-auto flex items-center justify-between gap-4">
            <div className="hidden lg:block">
              <p className="font-black text-lg">릴렉스드 와이드 슬랙스</p>
              <p className="text-red-500 font-bold">32,900원 <span className="text-gray-400 font-normal text-xs line-through ml-1">36,900</span></p>
            </div>
            <div className="flex flex-1 max-w-2xl gap-2">
              <button className="w-16 border border-zinc-300 flex items-center justify-center">
                <svg className="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg>
              </button>
              <button className="flex-1 bg-zinc-200 py-4 font-black hover:bg-zinc-300 transition">장바구니 담기</button>
              <button className="flex-[2] bg-black text-white py-4 font-black text-lg hover:opacity-90 active:scale-[0.98] transition">지금 바로 구매</button>
            </div>
          </div>
        </div>
      )}

      {/* 푸터 (사이트 하단) */}
      <footer className="bg-zinc-100 py-20 mt-40 border-t px-6 text-center text-gray-400 text-xs">
        <p className="mb-4 font-bold text-gray-600 uppercase tracking-widest text-sm">Musinsa Standard Clone Project</p>
        <p>© 2026 Musinsa Clone for A/B Testing Lab. All rights reserved.</p>
      </footer>
    </div>
  );
};

export default function App() {
  const [group, setGroup] = useState('A');

  return (
    <div className="antialiased">
      {/* 테스트 제어 패널 */}
      <div className="fixed top-20 right-6 z-[100] flex flex-col gap-2 scale-90 md:scale-100">
        <div className="bg-black text-white px-4 py-3 rounded-2xl shadow-2xl border border-zinc-700">
          <p className="text-[10px] text-zinc-400 uppercase font-black mb-2">A/B Testing Mode</p>
          <div className="flex gap-2">
            <button 
              onClick={() => setGroup('A')} 
              className={`px-3 py-1 rounded text-xs font-bold transition ${group === 'A' ? 'bg-blue-600 text-white' : 'bg-zinc-800 text-zinc-400'}`}
            >
              A안 (상단형)
            </button>
            <button 
              onClick={() => setGroup('B')} 
              className={`px-3 py-1 rounded text-xs font-bold transition ${group === 'B' ? 'bg-blue-600 text-white' : 'bg-zinc-800 text-zinc-400'}`}
            >
              B안 (하단고정)
            </button>
          </div>
        </div>
      </div>

      <ProductDetail testGroup={group} />
    </div>
  );
}
