# 현대중공업 기계사업부
9월 말 부터 투입 된 회사 프로젝트입니다. 현재 고객사측 사정으로 수정 진행 중에 있습니다.<br>
gulp 환경으로 진행되었으며, swiper.js, mousewheel.js, aos.js 등 다양한 프리소스를 사용하였습니다.

## Link
* https://gayoung914.github.io/hyundaidevserver/status/index_kor.html<br>
common/ mail/ customer service/ about us/ media 메뉴의 페이지들을 구현 하였습니다.

## Tool
* HTML5
* CSS3
* SCSS
* Jquery

## Skill
* About us - history 페이지 스크립트
  - **스크롤에 따라 활성화되는 점들과 progress bar**<br>
    👉 <img width="143" alt="image" src="https://user-images.githubusercontent.com/77196388/145222099-afef936a-8f5c-46b6-be55-853d213ae332.png"><br>
        인덱스 값 마다 길이 값을 가져와서 0번 째 값부터 n번째 까지 더한 길이가 활성화 점이 위치한 높이(=n번째 까지의 총 길이 합)보다 클 때 점이 활성화가 되도록 스크립트를 짜보았습니다.
```
 if ($line.height() > $dd.eq(0).height() + $dd.eq(1).height()) {
          $dd.eq(2).addClass("on");
          $dd.eq(2).addClass("active").siblings().removeClass("active");
        }

        if ($line.height() < $dd.eq(0).height() + $dd.eq(1).height()) {
          $dd.eq(2).removeClass("on");
        }

        if ($line.height() > $dd.eq(0).height() + $dd.eq(1).height() + $dd.eq(2).height()) {
          $dd.eq(3).addClass("on");
          $dd.eq(3).addClass("active").siblings().removeClass("active");
        }

        if ($line.height() < $dd.eq(0).height() + $dd.eq(1).height() + $dd.eq(2).height()) {
          $dd.eq(3).removeClass("on");
        }

        if ($line.height() > $dd.eq(0).height() + $dd.eq(1).height() + $dd.eq(2).height() + $dd.eq(3).height()) {
          $dd.eq(4).addClass("on");
          $dd.eq(4).addClass("active").siblings().removeClass("active");
        }
```
* ui.common.js 파일
  - **객체 지향적인 스크립트 정리 방식**<br>
    👉 함수 선언문, 객체 생성, 호이스팅 등을 활용하여 스크립트를 정리하였습니다.

## License
© HHI Engine & Machinery. All rights reserved.
