<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sonne Archive - 2026 Diary</title>
    <style>
        /* 전체 배경: 맥 OS 기본 월페이퍼 느낌의 그라데이션 */
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #e0c3fc 0%, #8ec5fc 100%);
            font-family: -apple-system, BlinkMacSystemFont, "SF Pro Text", "Helvetica Neue", Arial, sans-serif;
        }

        /* 사파리 브라우저 창 */
        .safari-window {
            width: 90%;
            max-width: 800px;
            height: 450px;
            background-color: #ffffff;
            border-radius: 12px;
            box-shadow: 0 30px 60px rgba(0,0,0,0.25);
            display: flex;
            flex-direction: column;
            overflow: hidden;
            border: 0.5px solid rgba(0,0,0,0.1);
        }

        /* 사파리 상단 툴바 */
        .toolbar {
            height: 50px;
            background: linear-gradient(to bottom, #f6f6f6, #ebebeb);
            display: flex;
            align-items: center;
            padding: 0 16px;
            border-bottom: 1px solid #d1d1d1;
            position: relative;
        }

        /* 왼쪽 상단 신호등 버튼 */
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

        /* 중앙 주소창 */
        .address-bar {
            margin: 0 auto;
            background-color: #ffffff;
            width: 60%;
            height: 28px;
            border-radius: 6px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 13px;
            color: #333;
            border: 1px solid #d1d1d1;
            box-shadow: 0 1px 2px rgba(0,0,0,0.05);
        }

        /* 본문 영역 */
        .content {
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-color: #fcfcfc;
        }

        /* 다이어리 제목 안내 */
        .title {
            margin-bottom: 30px;
            font-size: 24px;
            font-weight: 600;
            color: #333;
        }

        /* 다운로드 버튼: 모서리가 둥근 직사각형 */
        .download-btn {
            display: inline-block;
            padding: 16px 48px;
            background-color: #007aff; /* Apple Blue */
            color: white;
            text-decoration: none;
            font-size: 18px;
            font-weight: 500;
            border-radius: 12px;
            transition: all 0.2s ease;
            box-shadow: 0 4px 15px rgba(0, 122, 255, 0.3);
        }

        .download-btn:hover {
            background-color: #0063cc;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(0, 122, 255, 0.4);
        }

        .download-btn:active {
            transform: translateY(0);
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
                <span>yinseon.github.io/repository_for</span>
            </div>
        </div>
        
        <div class="content">
            <h1 class="title">2026 Diary Archive</h1>
            <a href="2026 diary.pdf" download="2026 diary.pdf" class="download-btn">
                다운로드
            </a>
        </div>
    </div>

</body>
</html>
