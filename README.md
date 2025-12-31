<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sonne Archive</title>
    <style>
        /* 배경 설정 */
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

        /* 16:9 비율을 유지하는 사파리 창 */
        .safari-window {
            width: 90vw; /* 화면 너비의 90% */
            aspect-ratio: 16 / 9; /* 16:9 비율 유지 */
            max-width: 1200px;
            background-color: #ffffff;
            border-radius: 12px;
            box-shadow: 0 30px 60px rgba(0,0,0,0.25);
            display: flex;
            flex-direction: column;
            overflow: hidden;
            border: 0.5px solid rgba(0,0,0,0.1);
        }

        /* 상단 툴바 */
        .toolbar {
            height: 50px;
            background: linear-gradient(to bottom, #f6f6f6, #ebebeb);
            display: flex;
            align-items: center;
            padding: 0 16px;
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
        .red { background-color: #ff5f56; border: 0.5px solid #e0443e; }
        .yellow { background-color: #ffbd2e; border: 0.5px solid #dea123; }
        .green { background-color: #27c93f; border: 0.5px solid #1aab29; }

        /* 주소창 (repository_for 삭제) */
        .address-bar {
            margin: 0 auto;
            background-color: #ffffff;
            width: 50%;
            height: 30px;
            border-radius: 6px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 14px;
            color: #333;
            border: 1px solid #d1d1d1;
        }

        /* 본문 중앙 정렬 */
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
            padding: 20px 60px;
            background-color: #007aff;
            color: white;
            text-decoration: none;
            font-size: 20px;
            font-weight: 500;
            border-radius: 14px;
            transition: all 0.2s ease;
            box-shadow: 0 4px 15px rgba(0, 122, 255, 0.3);
        }

        .download-btn:hover {
            background-color: #0063cc;
            transform: scale(1.05);
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
                <span>yinseon.github.io</span>
            </div>
        </div>
        
        <div class="content">
            <a href="2026 diary.pdf" download class="download-btn">
                Download 2026 Diary
            </a>
        </div>
    </div>

</body>
</html>
