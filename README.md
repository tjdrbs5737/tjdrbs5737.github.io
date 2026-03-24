import React, { useState, useEffect } from 'react';

const ProductPage = ({ testGroup }) => {
  const [scrollY, setScrollY] = useState(0);

  useEffect(() => {
    const handleScroll = () => setScrollY(window.scrollY);
    window.addEventListener("scroll", handleScroll);
    return () => window.removeEventListener("scroll", handleScroll);
  }, []);

  return (
    <div className="bg-white min-h-screen font-sans text-gray-900">
      {/* 상단 네비게이션 */}
      <nav className="sticky top-0 z-50 bg-white border-b p-4 flex justify-between items-center">
        <h1 className="font-black text-2xl tracking-tighter">MUSINSA CLONE</h1>
        <div className="space-x-4 text-sm font-bold">
          <span>SHOP</span>
          <span>LOOKBOOK</span>
          <span>COMMUNITY</span>
        </div>
      </nav>

      {/* 메인 상품 영역 */}
      <main className="max-w-6xl mx-auto flex flex-col md:flex-row p-6 gap-10">
        
        {/* 왼쪽: 상품 이미지 (길게 나열) */}
        <div className="w-full md:w-2/3 space-y-4">
          <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_5_500.jpg" alt="바지 메인" className="w-full" />
          <div className="bg-gray-100 p-8 text-center text-gray-500">
            <h3 className="text-xl font-bold mb-4">DETAIL INFO</h3>
            <p>여기에 무신사 스타일의 긴 상세 이미지가 들어갑니다.</p>
            <div className="h-[2000px] flex flex-col justify-around">
              <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_1_500.jpg" alt="상세1" />
              <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_2_500.jpg" alt="상세2" />
              <img src="https://image.msscdn.net/images/goods_img/20210316/1844582/1844582_3_500.jpg" alt="상세3" />
            </div>
          </div>
        </div>

        {/* 오른쪽: 구매 정보 사이드바 */}
        <div className="w-full md:w-1/3">
          <div className="sticky top-24 space-y-6">
            <div>
              <p className="text-sm text-gray-500 underline">[세미 와이드] 릴렉스 스테이트 슬랙스</p>
              <h2 className="text-2xl font-bold mt-2">무신사 스탠다드 릴렉스드 와이드 슬랙스</h2>
              <div className="flex items-center gap-2 mt-4">
                <span className="text-red-500 font-bold text-xl">10% OFF</span>
                <span className="text-2xl font-black">32,900원</span>
              </div>
            </div>

            {/* A안: 최상단 고정 구매 버튼 (스크롤해도 위에만 있음) */}
            {testGroup === 'A' && (
              <div className="flex flex-col gap-2">
                <button className="bg-black text-white py-4 font-bold hover:bg-gray-800 transition">바로 구매하기</button>
                <button className="border border-black py-4 font-bold hover:bg-gray-50">장바구니 담기</button>
              </div>
            )}

            <div className="border-t pt-4 text-sm space-y-2">
              <div className="flex justify-between"><span>적립금</span><span>최대 1,645원</span></div>
              <div className="flex justify-between"><span>배송비</span><span>무료배송</span></div>
            </div>
          </div>
        </div>
      </main>

      {/* B안: 따라다니는 플로팅 구매 버튼 (하단 고정바) */}
      {testGroup === 'B' && (
        <div className="fixed bottom-0 left-0 w-full bg-white border-t p-4 z-50 shadow-[0_-5px_15px_rgba(0,0,0,0.1)]">
          <div className="max-w-6xl mx-auto flex items-center justify-between gap-4">
            <div className="hidden md:block">
              <p className="text-xs text-gray-500">릴렉스드 와이드 슬랙스</p>
              <p className="font-bold">32,900원</p>
            </div>
            <div className="flex flex-1 gap-2">
              <button className="flex-1 bg-gray-200 py-3 font-bold">장바구니</button>
              <button className="flex-[2] bg-black text-white py-3 font-bold">지금 바로 구매</button>
            </div>
          </div>
        </div>
      )}
    </div>
  );
};

export default function App() {
  // 실제 A/B 테스트 환경에서는 URL 파라미터나 LocalStorage로 그룹을 나눕니다.
  const [group, setGroup] = useState('A');

  return (
    <div>
      <div className="fixed top-2 left-2 z-[100] bg-yellow-300 p-2 text-xs font-bold rounded shadow">
        현재 테스트 그룹: {group} 
        <button onClick={() => setGroup('A')} className="ml-2 underline">A형</button>
        <button onClick={() => setGroup('B')} className="ml-2 underline">B형</button>
      </div>
      <ProductPage testGroup={group} />
    </div>
  );
}
