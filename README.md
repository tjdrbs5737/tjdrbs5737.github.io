<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <meta name="mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <title>무신사 스타일 13.5oz 와이드 카고 팬츠 - 상품 상세</title>
    
    <script>
        (function() {
            // 브라우저의 로컬 스토리지 지원 여부를 안전하게 검증하는 방어적 코드
            function isLocalStorageSupported() {
                try {
                    var testKey = '__ab_test_support_check__';
                    window.localStorage.setItem(testKey, '1');
                    window.localStorage.removeItem(testKey);
                    return true;
                } catch (error) {
                    return false;
                }
            }

            if (isLocalStorageSupported()) {
                // 사용자가 이전에 방문하여 배정받은 실험 그룹(Bucket)이 있는지 확인
                var variant = window.localStorage.getItem('buy_button_ab_test_v1');
                
                // 로컬 스토리지에 데이터가 없다면(최초 방문자), 알고리즘을 통해 그룹 할당
                if (!variant) {
                    // Math.random()은 0 이상 1 미만의 난수를 반환. 50:50 확률로 A 또는 B 배정
                    variant = Math.random() >= 0.5? 'variant-a' : 'variant-b';
                    // 할당된 결과를 로컬 스토리지에 영구 저장 (Sticky Bucketing 구현)
                    window.localStorage.setItem('buy_button_ab_test_v1', variant);
                    
                    console.log(' 신규 사용자가 다음 모바일 웹 테스트 그룹에 배정되었습니다: ' + variant);
                } else {
                    console.log(' 기존 재방문 사용자 모바일 그룹 유지: ' + variant);
                }

                // 렌더링이 시작되기 전, 최상위 html 태그에 클래스를 주입하여 CSS 스위칭 준비 완료
                document.documentElement.classList.add(variant);
            } else {
                document.documentElement.classList.add('variant-a');
            }
        })();
    </script>

    <style>
        /* 모바일 웹 전용 기본 리셋 및 폰트 설정 */
        * { margin: 0; padding: 0; box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
            color: #333;
            line-height: 1.6;
            background-color: #fff;
            /* 모바일 스크롤 바운스 효과 및 스크롤 성능 최적화 */
            -webkit-overflow-scrolling: touch; 
            padding-top: 50px; /* 모바일 앱 바(헤더)가 차지하는 고정 공간 확보 */
        }

        /* 상단 모바일 앱 바 (App Bar) 구현 */
       .mobile-header {
            position: fixed; top: 0; left: 0; width: 100%; height: 50px;
            background: rgba(255, 255, 255, 0.95); backdrop-filter: blur(5px);
            border-bottom: 1px solid #eaeaea; display: flex; justify-content: space-between; align-items: center;
            padding: 0 15px; z-index: 10000;
            padding-top: env(safe-area-inset-top); /* iPhone 노치 영역 대응 */
            box-sizing: content-box;
        }
       .mobile-header h2 { font-size: 16px; font-weight: 600; color: #111; }
       .mobile-header button { background: none; border: none; font-size: 22px; color: #333; cursor: pointer; }

        /* 화면 100%를 차지하는 모바일 전용 콘텐츠 래퍼 */
      .product-container { width: 100%; overflow-x: hidden; background: #fff; }

        /* 무신사 레이아웃을 모방한 공통 섹션 여백 설정 */
        section { padding: 25px 15px; border-bottom: 1px solid #f0f0f0; }

        /* 이미지 반응형 처리 */
      .hero-section { padding-top: 15px; }
      .hero-section img { width: 100%; height: auto; display: block; margin-bottom: 15px; }

        /* 상품 기본 정보 타이포그래피 */
      .brand-name { font-size: 12px; color: #777; font-weight: bold; margin-bottom: 4px; display: block;}
      .product-title { font-size: 20px; font-weight: 700; margin-bottom: 10px; line-height: 1.3;}
      .product-price { margin-bottom: 15px; }
      .product-price del { color: #aaa; font-size: 14px; margin-right: 6px; }
      .product-price strong { font-size: 24px; color: #ff0000; letter-spacing: -0.5px; }
      .promo-box { background: #fdf5f5; border: 1px solid #ffdddd; color: #d0021b; padding: 10px; border-radius: 4px; font-size: 13px; margin-bottom: 10px; }

        /* AI 리뷰 요약 섹션 스타일링 */
      .ai-summary { background-color: #f8f9fa; padding: 20px; border-radius: 8px; }
      .ai-summary h3 { font-size: 14px; color: #000; margin-bottom: 8px; display: flex; align-items: center; }
      .ai-summary p { font-size: 13px; color: #444; word-break: keep-all; }

        /* 롱스크롤을 생성하는 더미 에디토리얼 박스 */
      .editorial-content {
            margin-top: 20px; background: linear-gradient(to bottom, #fafafa, #eaeaea);
            height: 2500px; display: flex; justify-content: center; align-items: flex-start;
            padding-top: 100px; color: #888; text-align: center; border-radius: 8px; border: 1px dashed #ccc; font-size: 13px;
        }
      .review-content {
            margin-top: 20px; background: #fff; height: 3000px; display: flex; justify-content: center;
            align-items: flex-start; padding-top: 100px; color: #888; border: 1px dashed #ccc; border-radius: 8px; font-size: 13px; text-align: center;
        }

        h3.section-title { font-size: 16px; margin-bottom: 12px; font-weight: 700; color: #111; }

        /* -------------------------------------------------------------
           A/B 테스트 동적 CSS 로직: 모바일 CTA 구매 액션 바 [31]
        ------------------------------------------------------------- */
        
        /* 액션 바의 뼈대 및 모바일 플렉스 박스 설정 */
      .action-bar {
            width: 100%; background: rgba(255, 255, 255, 0.98); backdrop-filter: blur(5px);
            z-index: 9999; display: flex; gap: 10px; padding: 12px 15px; transition: transform 0.3s ease; box-sizing: border-box;
        }

      .wish-btn {
            flex: 1; background: #fff; border: 1px solid #d9d9d9; border-radius: 6px;
            font-size: 20px; color: #555; cursor: pointer; padding: 12px 0;
        }

      .buy-btn {
            flex: 4; background: #000; color: #fff; border: none; border-radius: 6px;
            font-size: 15px; font-weight: bold; cursor: pointer; box-shadow: 0 4px 6px rgba(0,0,0,0.1); padding: 12px 0;
        }

        /* -------------------------------------------------------------
           Variant A 로직: 최상단 고정 인터페이스 (헤더 앱 바 바로 밑)
        ------------------------------------------------------------- */
        html.variant-a.action-bar {
            position: fixed;
            /* 헤더의 높이와 노치 영역을 더한 위치에 고정 */
            top: calc(50px + env(safe-area-inset-top)); 
            left: 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.06); border-bottom: 1px solid #eee;
        }

        /* Variant A일 경우 문서 전체를 버튼 높이(약 65px)만큼 추가로 아래로 밀어냄 */
        html.variant-a body {
            padding-top: calc(115px + env(safe-area-inset-top)); /* 50px(헤더) + 65px(버튼) */
        }

        /* -------------------------------------------------------------
           Variant B 로직: 하단 스크롤 동기화 플로팅 (엄지 영역 최적화) [31]
        ------------------------------------------------------------- */
        html.variant-b.action-bar {
            position: fixed;
            bottom: 0; 
            left: 0;
            box-shadow: 0 -2px 10px rgba(0,0,0,0.06); border-top: 1px solid #eee;
            /* iOS 홈 인디케이터 바를 침범하지 않도록 안전 영역 패딩 부여 */
            padding-bottom: calc(12px + env(safe-area-inset-bottom)); 
        }

        /* Variant B일 경우 하단의 리뷰 콘텐츠가 버튼에 가려지지 않도록 body 끝을 연장 */
        html.variant-b body {
            padding-bottom: calc(85px + env(safe-area-inset-bottom)); 
        }
    </style>
</head>
<body>

    <header class="mobile-header">
        <button aria-label="뒤로가기">←</button>
        <h2>상품 상세</h2>
        <button aria-label="장바구니">🛒</button>
    </header>

    <main class="product-container">
        
        <section class="hero-section">
            <img src="https://via.placeholder.com/800x1000/eeeeee/333333?text=Main+Lookbook+Image+Front" alt="와이드 카고 팬츠 전면 룩북 이미지">
            
            <span class="brand-name">TANSANMAGNESIUM</span>
            <h1 class="product-title">13.5oz 코튼 트윌 투턱 와이드 벌룬 카고 팬츠 [오트 밀크]</h1>
            
            <p class="product-price">
                <del>150,000원</del> 
                <strong>135,000원</strong>
            </p>
            
            <div class="promo-box">
                [앱 전용 혜택] 모바일 신규 가입 시 WLCMAPP 코드 입력으로 15% 추가 할인
            </div>
            
            <p style="font-size:13px; color:#555;">배송 정보: 한국에서 출고 / 평균 5~7일 이내 배송</p>
        </section>

        <section class="ai-summary-section">
            <div class="ai-summary">
                <h3>✨ AI 리뷰 요약 (Beta)</h3>
                <p>2,100만 건의 모바일 리뷰를 분석한 결과입니다. 허벅지부터 밑단까지 여유롭게 떨어지는 <strong>릴렉스한 레귤러 와이드 핏</strong>으로 캐주얼 및 시티보이 룩에 적합하다는 호평이 많습니다. <strong>13.5oz 두께의 100% 면 원단</strong>을 사용하여 한여름을 제외한 사계절 내내 착용이 가능합니다. 다만, 체형에 따라 <strong>기장이 다소 길게 느껴질 수 있다는 의견</strong>이 있으므로 구매 전 실측 사이즈를 반드시 확인하시기 바랍니다.</p>
            </div>
        </section>

        <section class="description-section">
            <h3 class="section-title">상품 상세 설명 (DESCRIPTION)</h3>
            <p style="font-size:13px; color:#444; line-height:1.7;">밑단에 3개의 다트(Dart)와 허리에 플리츠 디테일을 적용하여 입체적인 벌룬 실루엣을 구현했습니다. 밀도 높게 직조된 면 100% 트윌 원단은 가먼트 워싱(Garment washing) 처리를 거쳐 세탁 후의 수축과 이염을 최소화했습니다.</p>
            
            <div class="editorial-content">
                <p>[ 스크롤 2,500px 영역 ]<br><br>여기에 원단 클로즈업 사진, 봉제선 디테일 사진, <br>다양한 각도의 모델 착장 컷 10여 장이 <br>모바일 화면에 맞춰 연속 배치됩니다.<br><br>사용자는 스마트폰으로 이 이미지를 스와이프하며,<br>점차 구매 의사를 굳히게 됩니다.</p>
            </div>
        </section>

        <section class="size-guide-section">
            <h3 class="section-title">사이즈 및 핏 (SIZE & FIT)</h3>
            <p style="font-size:13px; color:#444;">모델 스펙: 1.82m / 70kg (30 사이즈 착용)</p>
            <div style="overflow-x: auto;">
                <table style="width:100%; margin-top:15px; border-collapse: collapse; font-size:12px; text-align:center;">
                    <tr style="background:#f4f4f4; border-top:2px solid #333; border-bottom:1px solid #ccc;">
                        <th style="padding:10px 5px;">사이즈</th><th style="padding:10px 5px;">총장</th><th style="padding:10px 5px;">허리</th><th style="padding:10px 5px;">밑위</th>
                    </tr>
                    <tr style="border-bottom:1px solid #eee;">
                        <td style="padding:10px 5px;">28</td><td style="padding:10px 5px;">102cm</td><td style="padding:10px 5px;">37cm</td><td style="padding:10px 5px;">31cm</td>
                    </tr>
                    <tr style="border-bottom:1px solid #eee;">
                        <td style="padding:10px 5px;">30</td><td style="padding:10px 5px;">104cm</td><td style="padding:10px 5px;">39.5cm</td><td style="padding:10px 5px;">32cm</td>
                    </tr>
                    <tr>
                        <td style="padding:10px 5px;">32</td><td style="padding:10px 5px;">106cm</td><td style="padding:10px 5px;">42cm</td><td style="padding:10px 5px;">33cm</td>
                    </tr>
                </table>
            </div>
        </section>

        <section class="review-section">
            <h3 class="section-title">포토 리뷰 (3,017건) <span style="color:#ff0000; font-size:13px; margin-left:8px;">★ 4.8 / 5.0</span></h3>
            
            <div class="review-content">
                <p>[ 스크롤 3,000px 영역 ]<br><br>수천 건의 모바일 포토 리뷰가 <br>무한 스크롤 형태로 로드되는 영역입니다.<br><br>엄지손가락으로 스와이프를 지속하던 사용자가<br>이 시점에 구매 버튼을 어디서 발견하는지가<br>전환율(CVR)을 결정짓는 핵심입니다.</p>
            </div>
        </section>

    </main>

    <div class="action-bar" id="purchase-action-bar">
        <button class="wish-btn" aria-label="찜하기">♡</button>
        <button class="buy-btn" id="btn-add-to-cart">구매하기</button>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            var buyButton = document.getElementById('btn-add-to-cart');
            
            buyButton.addEventListener('click', function() {
                var activeVariant = window.localStorage.getItem('buy_button_ab_test_v1') |

| 'unknown';
                
                console.log('[Analytics] 모바일 구매 버튼 클릭 이벤트!');
                console.log('- 배정된 Variant 속성: ' + activeVariant);
                console.log('- 모바일 스크롤 깊이: ' + window.scrollY + 'px');

                alert('A/B 테스트 추적 완료!\n\n현재 고객님이 배정된 테스트 그룹은 [' + activeVariant + '] 입니다.\n이 데이터는 분석 서버로 전송되어 통계 처리됩니다.');
            });
        });
    </script>
</body>
</html>
