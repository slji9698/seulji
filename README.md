<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>transform 연습5</title>
    <style>
        body{
            text-align: center;
            font-size: 20px;
        }
        .gallery{
            list-style: none;
            padding: 0;
            margin: 0 auto;
            width: 1260px;
        }
        .gallery li{/*420px*/
            width: 400px; height: 400px;
            float: left;
            margin: 10px;
            overflow: hidden;
        }
        .gallery .txt{
            background-color: rgba(0, 0, 0, 0.75);
            color: white;
            height: 400px;
            transition: 1s;
            
        }
        .gallery .txt h2{
            padding-top: 80px;/*마진상쇄현상-자식에게 마진 탑의 값을 주면 일반적인 흐름에서는 부모의 요소도 영향을 받는다. 둘 중 큰 값을 물려받음. 같이 딸려서 내려감. 이럴때, 일반적인 흐름을 만들지 않도록 만들자. overflow값을 넣으면 해결됨! overflow를 못넣겟다 싶으면 패딩을 넣어도 가능.*/
            margin: 0;
            
        }
        .gallery li:hover > .txt{
            transform: translateY(-400px);
            
        }
        .gallery li img{
            vertical-align: top;
        }
    </style>
</head>
<body>
    <h1>TRANS 연습 4</h1>
    <ul class="gallery">
        <li><img src="http://placehold.it/400x400" alt="임시이미지">
            <div class="txt">
                <h2>핸드폰케이스</h2>
                <p>설명이 어쩌고저쩌구</p>
                <p>가격: 20,500원</p>
            </div>
        </li>
        <li><img src="http://placehold.it/400x400" alt="임시이미지">
            <div class="txt">
                <h2>핸드폰케이스</h2>
                <p>설명이 어쩌고저쩌구</p>
                <p>가격: 20,500원</p>
            </div>
        </li>
        <li><img src="http://placehold.it/400x400" alt="임시이미지">
            <div class="txt">
                <h2>핸드폰케이스</h2>
                <p>설명이 어쩌고저쩌구</p>
                <p>가격: 20,500원</p>
            </div>ㄴ
        </li>
    </ul>
</body>
</html>
