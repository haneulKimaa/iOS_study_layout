> 🍎 iOS 레이아웃 뿌시기💪 <br> 
> 😎  개인 공부를 위한 프로젝트입니다!


## UIScrollView

### 주의 사항

> 💡 스크롤 뷰를 추가하고 위에 뷰를 올려 frame layout guide, content layout guide를 모두 붙여주고
반드시 뷰 내 콘텐츠의 위 아래를 지정한다. (스크롤뷰 높이를 지정해야 하기 때문)

<img width="335" alt="image" src="https://user-images.githubusercontent.com/63438947/160601326-88a43b43-be68-4db3-9427-f6a7c4b25a97.png">
<img width="432" alt="image" src="https://user-images.githubusercontent.com/63438947/160601361-8fe7f77b-ebe8-456a-8cd3-689683edbc5d.png">


### 1. Content Layout Guide

- 변형되지 않은 `스크롤뷰의 사각형 콘텐츠`를 기반으로 한다.
- __콘텐츠의 레이아웃을 잡을 때__ scroll view를 기준으로 잡는게 아니라 content layout guide를 잡아야 한다.
- 위에 올라갈 view는 content layout guide의 위아래좌우를 모두 잡아준다.

### 2. Frame Layout Guide

- 변형되지 않은 `프레임`을 기반으로 한 레이아웃 가이드.
- 스크롤을 가로로 할 것인지, 세로로 할 것인지 결정
    - 세로로 스크롤한다면 위에 뷰와 frame layout guide의 `width`를 맞춰준다.
