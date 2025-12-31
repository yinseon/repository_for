<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sonne Archive</title>
    <style>
        /* 기본 배경 설정 */
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #a1c4fd 0%, #c2e9fb 100%); /* 맥 배경 느낌의 그라데이션 */
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        /* 사파리 브라우저 창 스타일 */
        .safari-window {
            width: 80%;
            max-width: 900px;
            height: 500px;
            background-color: white;
            border-radius: 12px;
            box-shadow: 0 20px 50px rgba(0,0,0,0.2);
            display: flex;
            flex-direction: column;
            overflow: hidden;
        }

        /* 사파리 상단 툴바 */
        .toolbar {
            height: 45px;
            background-color: #ebebeb;
            display: flex;
            align-items: center;
            padding: 0 15px;
            border-bottom: 1px solid #d1d1d1;
        }

        /* 왼쪽 상단 신호등 버튼 (닫기, 최소화, 최대화) */
        .dots {
            display: flex;
            gap: 8px;
        }
        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
        }
        .red { background-color: #ff5f56; }
        .yellow { background-color: #ffbd2e; }
        .green { background-color: #27c93f; }

        /* 주소창 */
        .address-bar {
            flex-grow: 1;
            margin: 0 50px;
            background-color: white;
            height: 28px;
            border-radius: 6px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 13px;
            color: #666;
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

        /* 다운로드 버튼 스타일 */
        .download-btn {
            display: inline-block;
            padding: 15px 40px;
            background-color: #007aff; /* iOS/macOS 기본 파란색 */
            color: white;
            text-decoration: none;
            font-size: 18px;
            font-weight: 500;
            border-radius: 12px; /* 모서리가 둥근 직사각형 */
            transition: background-color 0.2s, transform 0.1s;
        }

        .download-btn:hover {
            background-color: #005ecb;
        }

        .download-btn:active {
            transform: scale(0.98);
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
                <span>sonne.archive</span>
            </div>
        </div>
        
        <div class="content">
            <a href="2026 diary.pdf" download class="download-btn">다운로드</a>
        </div>
    </div>

</body>
</html>
