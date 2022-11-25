# 221107
    <h3>Document.write() 활용</h3>
    
    <script>
        document.write('<h3>Welcome!</h3>');
        document.write('2+5는<br>');
        document.write('<mark>안녕하세요</mark>');
    </script>
    
    <script>
        function abc() {
            document.write('abcd');
            let res = eval("2*3 + 4*6");
            document.write('eval(\"2*3 + 4*6\")는' + res + '<br>');
            let m = parseInt("32");
            document.write('parseInt(\"32\")는' + m + '<br>');
            let n = parseInt("0x32");
            document.write('parseInt(parseInt(\"0x32\")는 ' + n + '<br>');
            n = parseInt("Hello");
            if (isNaN("10a"))
                document.write('숫자가 아닙니다.');
            else
                document.write('숫자입니다.');
        }
    </script>
    
    <h3>지역변수와 전역변수</h3>
    
    <script>
        var x = 100;
        //함수정의
        function f() {
            var x = 1;
            document.write('지역 변수 X =' + x) + "<br>";
            document.write('전역 변수 X =' + this.x);
        }
        //함수호출
        f();
    </script>
