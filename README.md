1번 문제

def list_students(*Names):
    for idx, name in enumerate(Names):
        print (idx, name)


list_students('한예슬','한시원','경진','배성윤')


# def list_students(**Names):


# 2번 문제

'''

mutable = 값이 변하는것
immutable = 값이 변하지 않는다는 의미

immutable => 숫자형(Number), 문자열(String), 튜플(Tuple)
mutable => 리스트(List), 딕셔너리(Dictionary)


* immutable/mutable 속성이 중요한 이유


'''



#3번 문제 DB Field에 사용되는 key 종류의 특징 서술하기

'''
CharField: 문자 사용가능 문자열의 길이를 한정
IntegerField: 숫자만 사용가능 
BooleanField: true, false값 사용가능
DateField: 파이썬 datetime.date 인스턴스에 의해 표현되는 날짜
FileField: 파일 업로드 필드 (ImageField)
TextField: 문자열의 길이를 한정하지 않는다
URLField: url을 위한 text field

OneToOneField vs ForeignKey vs ManyToManyField

OneToOneField 
-1:1관계에 사용됨. 하나의 항목에 여러개를 담을 수 없음


ManytoMany 필드는 다vs다 관계에서 사용됨.
-그래서 하나의 섹션에 여러개를 선택할 수 있음
-ManytoMany는 적용하면 하나의 테이블이 더 생긴다. 

'''
4. 

쿼리셋(QuerySet) : 데이터베이스에서 전달받은 '객체 목록' 리스트와 구조가 같지만 파이썬 기본 자료구조가 아니기때문에 파이썬에서 읽고 쓰기 위해선 자료형으로 변환(Casting)을 해줘야함 
object : 데이터베이스를 하나의 '객체' 덩어리로 봄
