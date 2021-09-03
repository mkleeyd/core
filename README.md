# core
toy_project_core

## 레이아웃 적용 후 컨텐츠 부분에 사용될 core html 코드
```
<!DOCTYPE html>
<html xmlns:th="http://www.thymeleaf.org"
      xmlns:layout="http://www.ultraq.net.nz/thymeleaf/layout"
      layout:decorator="~{layout/layout}">

<th:block layout:fragment="content">
    <!-- Begin Page Content -->
    <div class="container-fluid">
        <h1>레이아웃을 사용해 페이지 구성하기!</h1>
    </div>
</th:block>
</html>
```
- top, footer, sidebar 각 공통 html에 main.html 안에 있는 각 영역에 해당하는 코드부분 찾아서 넣어줌
- layout:decorator="~{layout/layout}":  기본 레이아웃을 layout/layout.html 파일을 사용하겠다라는 선언
- <th:block layout:fragment="content"> 아래에 코드를 작성하게 되면, layout.html에서 content라는 부분에 위치
- 각 파일마다 content 아래에 코드를 작성하시면서 개발 진행


