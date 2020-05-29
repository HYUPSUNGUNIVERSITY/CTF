#풀이

호스트와 포트를 받아 접속하면 뭐 별거 없는 웹사이트 하나가 나옵니다.

리스트를 누르면 flag.php와 json 어쩌구라는 두개의 하이퍼링크가 걸린 텍스트가 나오고, flag는 접속하면 deney됩니다.

이 flag.php 내용을 읽어야 하는데 문제파일을 다운받아 view.php의 내용을 보면, preg_match()를 이용해 flag라는 단어를 filtering하고있습니다.

구글 검색 결과 이 method를 bypass할 수 있는 여러가지 방법들이 발견되었지만, 실행해보니 전부 다 실패했습니다.

이를통해 view.php에서는 lfi취약점을 이용 할 수 없겠구나 싶어 main을 통해 flag를 얻을 수 있었습니.

그리고 이유는 모르겠지만 인코딩을 통해 값을 받지 않으면 can u see flag?라는 문자열이 보이고 real flag는 안보입니다

[] 