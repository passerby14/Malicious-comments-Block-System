# 기계학습 기반 문장분석을 통한 악의적인 댓글 선별

팀원 최봉근, 오민규, 설세형, 홍정우

요약 :2014년부터 2018년까지 사이버 명예훼손은 5년 동안 2배로 늘어났다. 이처럼 악의적인 댓글로 인한 피해는 점점 늘어나고 있는 추세이다. 하지만 많은 웹 사이트에서는 악의적인 댓글을 비속어를 키워드로 악의적인 댓글을 차단하거나 비속어에 해당하는 단어만 다른 언어 또는 xxx로 바꾸는 형식으로 차단하고 있다. 하지만 이런 차단방식은 비속어를 조금만 변경하면 이런 차단이 소용 없어지는 경우가 많다. 따라 서 우리는 단어의 의미를 벡터화하는 워드임베딩 기술을 이용하여 기존에 차단하지 못했던 이런 변형된 비속어나 줄임 말 등을 판별하여 악의적인 댓글인지 의심적인 댓글인지 일반적인 댓글인지를 분류한다.

자세한 사항은 문장을 분석하여 악의적인 댓글 선별.pdf 파일 참조<br>
논문: 기계학습_기반_문장분석을_통한_악의적인_댓글_선별.pdf

# 프로그램 다운받는곳 
https://drive.google.com/open?id=1KCOAHKQqeDcN0Qh68D_JbJcu0GDdmEA3

# 프로그램 사용방법 
1. Detecting-malicous-comments-senetence-analysis.zip파일을 다운 받아서 압축을 푼다
2. Detecting-malicous-comments-senetence-analysis파일안에 있는 detecting.exe를 실행 시킨다
3. 프로그램을 실행 시키고 조금 기다리면 'url을 입력하세요'라는 문구와 함께 창이 뜬다 이때 네이버 뉴스 url을 입력해주고 ok를 누른다
4. keyword를 입력하라는 문구가 나온다. keyword를 입력하고 ok를 누른다 만약 keyword를 입력하지 않을려면 빈칸으로 ok를 누른다.
5. 조금 기다리면 댓글 총개수와 악플 개수 의심개수 일반 개수를 보여준다음 프로그램이 종료되었습니다라는 문구가 뜬다.
6. 파일안에 총 댓글과 악플,의심,일반txt파일이 생성 되어있다.

# 프로그램 시연 동영상
키워드가 없을시 :https://www.youtube.com/watch?v=PRDsxupsVSI&feature=youtu.be <br>
키워드가 있을시 :https://www.youtube.com/watch?v=VLx0hKOC9ag&feature=youtu.be <br>
더 많은 시연영상은 '문장을 분석하여 악의적인 댓글 선별.pdf' 파일 결론부분이 있습니다.

# 제작기간
2019-04-11 ~ 2019-12-10<br>
crawler가 붙은 파일들은 모델을 학습시키기 위해 크롤링하기 위해 사용했던 코드<br>
keyword.py gui없는 버전의 코드<br>
detecting.py gui있는 버전의 코드<br>

ps. morphological analysis 파일안에는 형태소 분석기 정확도 분석을 실시하였다. <br> 
초반에는 형태소분석기를 사용하여 단어 토큰화 하여 사용할 목적으로 <br>
형태소 분석기 정확도 분석을 실시하였으나 fastText를 사용하는 바람에 사용하지 않았다. <br>
분석 결과는 morphological analysis 파일안 형태소 분석기 비교.pdf 참고
