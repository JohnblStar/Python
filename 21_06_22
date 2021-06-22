import time
import random
import datetime
HARD = {'상상더하기': '''1, 2 Come On, R U Ready
3, 4 Do It I'm Ready
5, 6 Baby Are You Ready
지금 나와 어디든 가자
지루한 하루 여기까지만 All Stop
작은 가방 운동화 챙겨
자 더 크게 Radio를 높이고
코발트블루 물결 눈부신 바다
달빛 가득 묻은 작은 섬
야경이 눈부신 도시는 어때?
함께라면 어디든 좋아
난 너와 나 그곳으로
떠나는 거야
상상에 상상에 상상을 더해서
어머 깜짝야
눈부셔 눈부셔 눈부셔 이건 뭐
Oh Hello New World
두 손 모아 소리치면
푸른 하늘이 내게로 와
날아가볼래
상상의 상상의 미래로 가볼까
바람을 타고
새로운 눈빛에 가슴이 붐 붐 붐
Oh 발견했어 우리들만의 Paradise
흑백영화 같은 하루에
레몬 터지듯 짜릿함이 필요해
지금 당장 널 데려갈게
꿈꿔오던 사진 속 그곳으로
민트그린빛 바람 가득한 숲 속
달콤한 향기의 칵테일
지도를 벗어나 Ticket To The Dream
함께라면 어디든 좋아
난 너와 나 그곳으로
떠나는 거야
상상에 상상에 상상을 더해서
어머 깜짝야
눈부셔 눈부셔 눈부셔 이건 뭐
Oh Hello New World
두 손 모아 소리치면
푸른 하늘이 내게로 와
날아가볼래
상상의 상상의 미래로 가볼까
바람을 타고
새로운 눈빛에 가슴이 붐 붐 붐
Oh 발견했어 우리들만의 Paradise
너와 나의 비밀스런 풍경들
언제라도 다시 와 주겠니
은하수 아래 밤새 부른 노래
영원히 잊지 않을 거야
이 시간 속에 영원히
네 품에 안기고 싶은걸
단 둘이 이순간 잠들고 싶은걸
지도엔 없는 이 곳을 꼭 기억해줘
우리들만의 Paradise
상상에 상상에 상상을 더해서
어머 깜짝야
눈부셔 눈부셔 눈부셔 이건 뭐
Oh Hello New World
처음 만난 세상 속에
나의 가슴이 라 라 라 라
날아가볼래
상상의 상상의 미래로 가볼까
바람을 타고
새로운 눈빛에 가슴이 붐 붐 붐
Oh 발견했어 우리 들만의 Paradise
1, 2 Come On, R U Ready
3, 4 Do It I'm Ready
5, 6 Baby Are You Ready
''',
        '롤린': '''그 날을 잊지 못해 babe
날 보며 환히 웃던 너의 미소에
홀린 듯 I'm fall in love
But 너무 쪽팔림에 (난 그저)
한마디 말도 못해 babe
I wanna you 너의 눈빛은
날 자꾸 네 곁을 맴돌게 해
Just only you 굳게 닫힌 내 맘이
어느새 무너져버려 Because of you
온통 너의 생각뿐이야 나도 미치겠어
너무 보고 싶어 매일 매일 매일
자꾸 초라해지잖아 내 모습이
그대여 내게 말해줘 사랑한다고
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
하루가 멀다 하고 Rolling in the deep
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
기다리고 있잖아 Babe Just only you
기다리고 있잖아 Babe Just only you
Hey I just wanna be with you
오늘 밤이 가기 전에
I can't feel you 조금 더 다가와 줘
Tonight I'm ready for you
You wanna touch me I know
대체 뭘 고민해 빨리 안아
아닌 척 모르는 척 하다가
늦게 놓치고 후회 말아
I wanna you 너의 눈빛은
날 자꾸 네 곁을 맴돌게 해
Just only you 굳게 닫힌 내 맘이
어느새 무너져버려 Because of you
온통 너의 생각뿐이야 나도 미치겠어
너무 보고 싶어 매일 매일 매일
자꾸 초라해지잖아 내 모습이
그대여 내게 말해줘 사랑한다고
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
하루가 멀다 하고 Rolling in the deep
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
기다리고 있잖아 Babe Just only you
이제 와 숨기려 하지 마요
그대여 아닌 척하지 마요
온종일 난 그대 생각에 잠긴 채로
난 이대로 기다리고 있어요
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
하루가 멀다 하고 Rolling in the deep
Rollin' Rollin' Rollin' Rollin'
Rollin' Rollin' Rollin' Rollin'
기다리고 있잖아 Babe Just only you
기다리고 있잖아 Babe Just only you
        '''
}
MID = {'가족사진':'''바쁘게 살아온 당신의 젊음에
의미를 더해줄 아이가 생기고
그날에 찍었던 가족 사진속에
설레는 웃음은 빛바래 가지만
어른이 되어서 현실에 던져진
나는 철이없는 아들이 되어서
이곳저곳에서 깨지고 또 일어서다
외로운 어느날 꺼내본 사진속
아빠를 닮아있네
내 젊은 어느새 기울어 갈때쯤
그제야 보이는 당신의 날들이
가족사진속에 미소띤 젊은 아가씨에
꽃피던 시절은 나에게 다시 돌아와서
나를 꽃피우기 위해 거름이 되어버렸던
그을린 그 시간들을 내가 깨끗히 모아서
당신의 웃음 꽃 피우길
    ''',
       '가시': '''너 없는 지금도 눈부신 하늘과
눈부시게 웃는 사람들
나의 헤어짐을 모르는 세상은
슬프도록 그대로인데
시간마저 데려가지 못하게
나만은 널 보내지 못했나봐
가시처럼 깊게 박힌 기억은
아파도 아픈줄 모르고
그대 기억이 지난 사랑이
내 안을 파고 드는 가시가 되어
제발 가라고 아주 가라고
애써도 나를 괴롭히는데
아픈만큼 너를 잊게 된다면
차라리 앓고 나면 그만인데
가시처럼 깊게 박힌 기억은
아파도 아픈 줄 모르고
제발 가라고 아주 가라고
애써도 나를 괴롭히는데
너무 사랑했던 나를
크게 두려웠던 나를
미치도록 너를 그리워했던
날 이제는 놓아줘
보이지 않아 내 안에 숨어
잊으려 하면 할수록 더 아파와
제발 가라고 아주 가라고
애써도 나를 괴롭히는데
'''
}
LOW = {'라라라': '''그대는 참 아름다워요 밤 하늘의 별빛보다 빛나요
지친 나의 마음을 따뜻하게 감싸줄
그대 품이 나의 집이죠
세찬 바람 앞에서 꺼질듯한 내 사랑도
잘 참고서 이겨내줬어요
정말 눈물나도록 고마운 맘 아나요
그대 내곁에 살아줘서
사랑해요 사랑해요 내가 그대에게 부족한걸 알지만
세월을 걷다보면 지칠 때도 있지만
그대의 쉴곳이 되리라 사랑해요 고마운 내 사랑
평생 그대만을 위해 부를 이 노래
사랑 노래 함께 불러요 둘이서 라랄라
그대 쳐진 어깨가 내맘을 아프게 해요
잘 해준것도 없는 나라서
그대의 고운 손이 세월에 변했어요
못지켜줘서 미안해요
사랑해요 사랑해요 내가 그대에게 부족한걸 알지만
세월을 걷다보면 지칠때도 있지만
그대에게 쉴곳이 되리라 사랑해요 고마운 내 사랑
평생 그대만을 위해 부를 이노래
사랑노래 함께 불러요 둘이서 라랄라
고마워요 고마워요 그대 자신보다 나를 아껴준 사랑
세상이 등 돌려도 누가 뭐라고 해도
내가 그대 지켜줄게요
사랑해요 소중한 내사랑
평생 그대만을 위해 부를 이노래
사랑노래 함께 불러요 둘이서 라라라
그대 품이 나의 집이죠 영원히 라라라
''',
       '살다가':'''살아도 사는게 아니래
너 없는 하늘에 창 없는 감옥같아서
웃어도 웃는게 아니래
초라해 보이고 우는것 같아 보인대
사랑해도 말 못했던 나
내색 조차 할 수 없던 나
나 잠이드는 순간 조차 그리웠었지
살다가 살다가 살다가 너 힘들 때
나로 인한 슬픔으로 후련할 때까지
울다가 울다가 울다가 너 지칠 때
정 힘들면 단 한번만 기억하겠니
살다가
웃어도 웃는게 아니래
초라해 보이고 우는 것 같아 보인대
사랑해도 말 못했던 나
내색 조차 할 수 없던 나
나 잠이드는 순간 조차 그리웠었지
살다가 살다가 살다가 너 힘들 때
나로 인한 슬픔으로 후련할 때까지
울다가 울다가 울다가 너 지칠 때
정 힘들면 단 한번만 기억하겠니
우리 마지못해 웃는거겠지
우리 마지못해 살아가겠지
내 곁에 있어도
너의 곁에 있어도 눈물나니까
살다가 살다가 살다가 너 힘들 때
나로 인한 슬픔으로 후련할 때까지
태워도 태워도 태워도 남았다면
남김없이 태워도돼 후련할 때까지
나 살다가
나 살다가
       '''
}
sec = input
class Tajagame:
    '''
    - 사용자 이름, 난이도 입력 받기
    '''
    def __init__(self):
        self.player = input("플레이어 이름: ")
        self.level()
        self.count()
        self.start()
    '''
    - 시작한다는 내용 프린트
    - 카운트 다운
    '''
    def start(self):
        '''
        카운트다운 실행
        가사를 하나씩 띄우기
        '''
        time_log = []
        tasok_log = []
        acc_log = []
        if self.lev == 'high':
            candidate = HARD
        elif self.lev == 'middle':
            candidate = MID
        elif self.lev == 'low':
            candidate = LOW
        # random.choice(list(candidate.values()))
        question = random.choice(list(candidate.items()))
        # print(f'제목 : {question[0]} \n가사 : {question[1]}')

        lyrics = question[1]
        lyrics = lyrics.split("\n")

        for lc in lyrics:

            start= datetime.datetime.now() #시작 시간
            print('가사:',lc) #가사 표시
            inp = input('작성: ') #타자작성 시 받아오는 값
            elapsed = datetime.datetime.now() - start #종료시간
            time_log.append(elapsed.total_seconds())

            if inp == lc:
                print('잘 진행 중')
            else:
                cnt = 0
                print('오타다!!')
                for li1, li2 in zip(lc, inp):
                    if li1 == li2: cnt+=1
                aim = cnt / len(lc)  # 정확도 체크
                acc_log.append(aim)
                print(cnt, aim*100)
            tasok = len(inp)/elapsed.total_seconds()*60
            tasok_log.append(tasok)
            # speed = tasu / elapsed.total_seconds()
            print(tasok)
        AVG_acc = sum(acc_log)/len(acc_log)
        AVG_tasok =sum(tasok_log)/len(tasok_log)
        AVG_time =sum(time_log)/len(time_log)
        print(AVG_acc)
        print(AVG_tasok)
        print(AVG_time)

        # print('선택 난이도에 high, middle, low 중 하나를 입력하세요')
    def level(self):
        lev = input("선택 난이도: ")
        while lev not in ['high', 'low', 'middle']:
            print('땡!!! 선택 난이도를 high, low, middle 중에서만 선택하세요')
            lev = input("선택 난이도: ")
        if lev=='high': print(f'현재 난이도는 *high*')
        elif lev == 'low': print('현재 난이도는 *low*')
        elif lev == 'middle': print('현재 난이도는 *middle*')
        self.lev = lev

    def count(self):
        print('시작합니다!!')
        sec = 2
        while sec != 1:
            sec -= 1
            print(sec)
            time.sleep(1)

game = Tajagame()
