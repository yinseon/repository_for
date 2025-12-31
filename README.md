<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sonne Archive</title>
    <style>
        /* 1. 깃허브 기본 테마 요소(글씨, 선) 숨기기 */
        header, footer, .sidebar, .header-inner {
            display: none !important;
        }

        /* 배경 및 기본 설정 */
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #e0c3fc 0%, #8ec5fc 100%);
            font-family: -apple-system, BlinkMacSystemFont, "SF Pro Text", sans-serif;
        }

        /* 16:9 비율의 사파리 창 */
        .safari-window {
            width: 90vw; 
            aspect-ratio: 16 / 9; 
            max-width: 1100px;
            background-color: #ffffff;
            border-radius: 12px;
            box-shadow: 0 30px 60px rgba(0,0,0,0.25);
            display: flex;
            flex-direction: column;
            overflow: hidden;
            /* 2. 사파리 테두리 외의 선 제거 */
            border: none; 
        }

        /* 상단 툴바 */
        .toolbar {
            height: 45px;
            background: linear-gradient(to bottom, #f6f6f6, #ebebeb);
            display: flex;
            align-items: center;
            padding: 0 16px;
            /* 3. 툴바 하단 선 (원치 않으시면 'none'으로 변경 가능) */
            border-bottom: 1px solid #d1d1d1;
            position: relative;
            flex-shrink: 0;
        }

        /* 신호등 버튼 */
        .dots {
            display: flex;
            gap: 8px;
            position: absolute;
            left: 16px;
        }
        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
        }
        .red { background-color: #ff5f56; }
        .yellow { background-color: #ffbd2e; }
        .green { background-color: #27c93f; }

        /* 주소창 (sonne math로 변경) */
        .address-bar {
            margin: 0 auto;
            background-color: #ffffff;
            width: 45%;
            height: 26px;
            border-radius: 6px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 13px;
            color: #333;
            border: 1px solid #d1d1d1;
        }

        /* 본문 영역 */
        .content {
            flex-grow: 1;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #fafafa;
        }

        /* 다운로드 버튼 (모서리가 둥근 직사각형) */
        .download-btn {
            display: inline-block;
            padding: 18px 50px;
            background-color: #007aff;
            color: white;
            text-decoration: none;
            font-size: 18px;
            font-weight: 500;
            border-radius: 12px;
            transition: all 0.2s ease;
            box-shadow: 0 4px 15px rgba(0, 122, 255, 0.2);
        }

        .download-btn:hover {
            background-color: #0063cc;
            transform: translateY(-2px);
        }
    </style>
</head>
<body>

    <div class="safari-window">
        <div class="toolbar">
            <div class="dots">
                <div class="dot red"></div>
                <div class="dot yellow"></div>
                <div class="dot green"></div>
            </div>
            <div class="address-bar">
                <span>sonne math</span>
            </div>
        </div>
        
        <div class="content">
            <a href="2026 diary.pdf" download class="download-btn">
                다운로드
            </a>
        </div>
    </div>

</body>
</html>
