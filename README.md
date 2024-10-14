<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <style>
        @font-face {
            font-family: 'RixXladywatermelonR';
            src: url('https://fastly.jsdelivr.net/gh/projectnoonnu/2408-4@1.0/RixXladywatermelonR.woff2') format('woff2');
            font-weight: normal;
            font-style: normal;
        }

        .text {
            font-family: 'RixXladywatermelonR'; /* 폰트 패밀리 추가 */
            font-size: 50px;
            text-align: center;
            margin-top: 12%;
            margin-bottom: 6%;
            user-select: none; /* 텍스트 드래그 방지 */
        }

        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
        }

        body {
            display: flex;
            flex-direction: column;
            align-items: center; /* 수평 중앙 정렬 */
            background-image: url("홈화면_배경.jpg");
            background-size: contain;
            background-position: center;
            background-repeat: no-repeat; /* 이미지 반복 제거 */
            height: 100vh;
        }

        .button {
            font-family: 'RixXladywatermelonR'; /* 폰트 패밀리 추가 */
            font-size: 30px; /* 글자 크기 */
            text-align: center;
            background-color: #f9ed89; /* 버튼 배경색 */
            color: #333; /* 글자 색상 */
            padding: 10px 15px; /* 버튼 안의 여백 줄임 (가로 줄임) */
            margin: 10px; /* 버튼 간의 간격 */
            border: none; /* 테두리 없애기 */
            border-radius: 5px; /* 모서리 둥글게 하기 */
            cursor: pointer; /* 커서 모양 변경 */
            transition: background-color 0.3s; /* 호버 효과 부드럽게 */
            width: 150px; /* 버튼의 고정 가로 크기 */
            user-select: none; /* 버튼 드래그 방지 */
        }

        .button:hover {
            background-color: #ff8e5e66; /* 호버 시 배경색 변경 */
        }
    </style>
</head>
<body>
    <div class="text">민들레<br> 홀씨의 모험</div>
    <div class="button" id="startButton">시작</div>
    <div class="button" id="instructionsButton">게임방법</div>

    <script>
        // "시작" 버튼을 클릭하면 다음 페이지로 이동
        document.getElementById("startButton").onclick = function() {
            window.location.href = "1.html"; // 이동할 HTML 파일 경로
        };

        // "게임방법" 버튼도 다른 페이지로 이동하게 할 수 있음
        document.getElementById("instructionsButton").onclick = function() {
            window.location.href = "게임방법.html"; // 게임 방법 페이지로 이동
        };
    </script>

</body>
</html>
