<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <div id="bai1">
        <h5>bài 1:</h5>
        <button class="btn-bai1">bai1</button>
    </div>
    <div id="bai2">
        <h5>bài 2:</h5>
        <button class="btn-bai2">Welcome</button>
        <input type="text" placeholder="Welcome to" class="inputName2">
    </div>
    <div id="bai3">
        <h5>Bài 3:</h5>
        <button class="btn-bai3">Welcome</button>
        <input type="text" placeholder="Welcome to" class="inputName3">
        <input type="text" placeholder="kết quả" class="result">
    </div>
    <div id="bai4">
        <h5>Bài 4:</h5>
        <label>Năm sinh:</label>
        <input type="text" placeholder="Nhập Năm sinh" class="year">
        <button class="resultEx4">Tính</button>
        <label>Tuổi:</label>
        <input type="text" class="old">
    </div>
    <div id="bai6" width="100%" height="100px">
        <h5>Bài 6: </h5>
        <button class="blue" style="color: blue;">Blue</button>
        <button class="red" style="color: red;">Red</button>
    </div>
    <div id="bai7" width="100%" height="100px">
        <h5>Bài 7:</h5>
        <select class="selector">
            <option value="do" style="color: red;">Red</option>
            <option value="xanhduong" style="color: blue;">Blue</option>
            <option value="xanhla" style="color: green;">Green</option>
            <option value="vang" style="color: yellow;">Yellow</option>
        </select>
        <button class="btn-bai7">Chọn</button>
    </div>
    <div id="bai12">
        <h5>Bài 12:</h5>
        <label>Số lượng:</label>
        <input type="text" class="inputsoluong" placeholder="số lượng">
        <br>
        <label>Đơn giá:</label>
        <input type="text" class="inputdongia" placeholder="đơn giá">
        <br>
        <button class="tinh">Tính</button>
        <br>
        <label>Thành tiền:</label>
        <input type="text" class="outputthanhtien" placeholder="thành tiền">
    </div>
    <div id="bai13">
        <h5>bài 13:</h5>
        <button type="button" class="btn-start">Start</button>
        <button type="button" class="btn-stop">Stop</button>
        <button type="button" class="btn-reset">Reset</button>
        <h3 id="display"><time>00:00:00:000</time></h3>
    </div>
    <div id="bai9">
        <h5>bài 9:</h5>
    </div>
    <div id="bai5">
        <h5>Bài 5: yêu cầu nhập lại nếu năm sinh > năm</h5>
        <label>Nhập năm sinh:</label>
        <input type="text" class="date" placeholder="nhập năm sinh">
        <button class="btn-bai5">Kiểm tra</button>
    </div>
    <script src="BaiTapDom.js"></script>
</body>
</html>