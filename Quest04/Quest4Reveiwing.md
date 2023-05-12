
# Code Peer Review Templete
- 코더 :  백기웅 님
- 리뷰어 :  박동원



# PRT(PeerReviewTemplate)
각 항목을 스스로 확인하고 체크하고 확인하여 작성한 코드에 적용하세요.
- [x] 1.코드가 정상적으로 동작하나요?
- [x] 2.문제를 제대로 이해했나요?
- [x] 3.함수가 작동하는 방식을 잘 설명했나요?
- [x] 4.발생 가능한 에러를 찾아서 디버깅을 했나요?
- [x] 5.코드를 더 개선시켰나요?


# 코드
```python
import random
import time           # 이 부분은 왜 가져 오셨는지 잘 모르겠습니당 


class Fish:
  def __init__(self, name, speed):
    self.name = name
    self.speed = speed         # 클래스 잘 만들어 주셨네요. 전 아직 노드 안공부해서 클래스 만드는법 잘 배우고 갑니당

fish_list = [
    Fish("Nemo", 3),
    Fish("Dory", 5),
    Fish("Marlin", 7),
    Fish("Bubbles", 2),
    Fish("Gill", 4)
]                                     # 입력값, 입력 값이 앞에 나와 있군요 ㅎㅎ


def show_fish_movement_comprehension(fish_list):
  [print(f"{fish.name} is swimming at {fish.speed} m/s") for fish in fish_list]      #컨프리헨션 안에 문장완성 시키 셨군요

print("Using Comprehension:")                                  # 출력값  잘 확인 됩니다
show_fish_movement_comprehension(fish_list)



def show_fish_movement_iterator(fish_list):                # 이터레이터 만드게 liter() 이렇게 인걸 로 알고 있는데.. 아닌가여?
    for fish in fish_list:
      print(f"{fish.name} is swimming at {fish.speed} m/s")

print("Using Iterator: ")              # 출력값 잘 확인 됩니다.
show_fish_movement_iterator(fish_list)


def show_fish_movement_iterator(fish_list):
  def fish_movement_generator():                                  # 제너레이터 부분 완성 하시면 다시 보러 오겠습니다
    for fish in fish_list:
      yield f"{fish.name} is swimming at {fish.speed} m/s" 

      print(f"{fish.name} is swimming at {fish.speed} m/s")

print("Using Iterator: ")
show_fish_movement_iterator(fish_list)

```

# 리뷰
코드 리뷰 이상입니다 너무 잘 하셨구요<br/>
클래스 부분 잘 배우고 갑니다<br/>
제너레이터 부분 완성 되시면 다시 리뷰하러 오겠습니다<br/>
수고하셨습니다<br/>
제너레이터 꿀팁<br/> https://dojang.io/mod/page/view.php?id=2412 <br/>여기 참고 해보시죠

