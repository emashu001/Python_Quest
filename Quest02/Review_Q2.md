# Code Peer Review Templete

- 코더 : 백기웅
- 리뷰어 : 김태원

---

# PRT(PeerReviewTemplate)

- [o] 코드가 정상적으로 동작하고 주어진 문제를 해결했나요?
- [o] 주석을 보고 작성자의 코드가 이해되었나요?
- [o] 코드가 에러를 유발할 가능성이 있나요?
- [o] 코드 작성자가 코드를 제대로 이해하고 작성했나요? (직접 인터뷰해보기)
- [o] 코드가 간결한가요?

---

# 코드.
<pre>
<code>
maze = [
    [0, 1, 0, 0, 0],
    [0, 0, 0, 1, 0],
    [0, 1, 1, 0, 0],
    [0, 0, 1, 1, 0],
    [0, 0, 0, 0, 0]
]

# print(turtle start point :, maze[x][y])

def findroad(x, y):
  if maze[x][y] == 0:
    print(길이 yes!)
    # x += 1
    maze[x][y] = 2
    print (tutle now point :,  (x, y), maze[x][y])

  elif maze[x][y] == 1:
    print(길이 no, 좌표를 다시 적어 주세요!)
    print (tutle now point :,  (x, y), maze[x][y])
     

for x in range(len(maze)):
  for y in range(len(maze)):
    findroad(x,y)

maze
</code>
</pre>


---
#코드리뷰
- turtle 라이브러리를 활용하여 시각화는 하지 못하였지만 벽과 길을 구분하는 경로탐색은 성공했습니다.
- 좌표에서 벽(1)을 만났을때, break으로 elif문을 빠져나가 다음행을 탐색할 수 있도록 해야 합니다.
- 시각화 후에는 벽(1)을 만났을때 왔던 길로 되돌아가는 로직도 필요할것 같습니다.
# 참고 링크 및 코드 개선 여부

<pre>
<code>
elif maze[x][y] == 1:
    print(길이 no, 좌표를 다시 적어 주세요!)
    print (tutle now point :,  (x, y), maze[x][y])
    break # 탈출
</code>
</pre>
