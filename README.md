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
- 상단에 layout:decorator="~{layout/layout}" 은 기본 레이아웃을 layout/layout.html 파일을 사용하겠다라는 선언하는 것 입니다.
- <th:block layout:fragment="content"> 아래에 코드를 작성하게 되면, layout.html에서 content라는 부분에 위치하도록 합니다.
- 각 파일마다 content 아래에 코드를 작성하시면서 개발을 하시면 됩니다.


