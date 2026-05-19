<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bài Lab 5 - jQuery Ẩn/Hiện</title>
    
    <script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
    
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 50px;
            background-color: #f9f9f9;
        }
        h2 {
            color: #2b5797;
        }
        .btn-group button {
            padding: 8px 15px;
            margin-right: 5px;
            background-color: #f0f0f0;
            border: 1px solid #ccc;
            cursor: pointer;
            border-radius: 3px;
        }
        .btn-group button:hover {
            background-color: #e0e0e0;
        }
        #content-box {
            margin-top: 20px;
            padding: 20px;
            width: 300px;
            background-color: #d1ecf1;
            border: 2px solid #17a2b8;
            border-radius: 4px;
            color: #0c5460;
        }
        #content-box h4 {
            margin-top: 0;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <h2>Bài tập jQuery Ẩn / Hiện nội dung</h2>
    <div class="btn-group">
        <button id="btn-hide">Ẩn nội dung</button>
        <button id="btn-show">Hiện nội dung</button>
        <button id="btn-toggle">Ẩn / Hiện</button>
    </div>
    <div id="content-box">
        <h4>Thông báo</h4>
        <p>Đây là nội dung được điều khiển bằng jQuery.</p>
    </div>
    <script>
        $(document).ready(function() {
            $("#btn-hide").click(function(){
                $("#content-box").hide(400);
            });
            $("#btn-show").click(function(){
                $("#content-box").show(400);
            });
            $("#btn-toggle").click(function(){
                $("#content-box").toggle(400);
            });
        });
    </script>

</body>
</html>
