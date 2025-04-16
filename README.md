##반응형 global.scss 참고.

| Mobile    | Tablet     | Desktop   | class             |
| ------    | ------     | -------   | ----------------- |
| O         | X          | X         |    `.sm-only`     |
| O         | O          | X         |    `.lg-hidden`   |
| X         | O          | X         |    `.md-only`     |
| X         | O          | O         |    `.sm-hidden`   |
| X         | X          | O         |    `.lg-only`     |
| O         | X          | O         |    `.md-hidden`   |




### 1. GNB

- 로그인을 하지 않은 경우

```html

              <div class="button-group">
                <button class="lg-hidden gnb-icon-button is-search" 
                type="button" aria-label="검색창열기버튼">
                  <i class="ico_search" ></i>
                </button>
                <a class="gnb-icon-button is-cart" href="/" aria-label="장바구니 페이지 이동">
                  <i class="ico_cart"></i>
                  <!-- <strong class="badge">5</strong> -->
                </a>
                <div class="sm-hidden gnb-auth">
                  <a href="#">로그인</a>
                  <a href="#">회원가입</a>  
                </div>
              </div>

```
- 로그인을 한 경우

```html

          <div class="button-group">
                <button class="lg-hidden gnb-icon-button is-search active gnb-search-button" 
                type="button" aria-label="검색창열기버튼">
                  <i class="ico_search" ></i>
                </button>
  
                <a class="sm-hidden gnb-icon-button" href="/" aria-label="스크랩북 페이지 이동">
                  <i class="ico_bookmark"></i>
                </a>
  
                <a class="sm-hidden gnb-icon-button" href="/" aria-label="내소식 페이지 이동">
                  <i class="ico_bell"></i>
                </a>
  
                <a class="gnb-icon-button is-cart" href="/" aria-label="장바구니 페이지 이동">
                  <i class="ico_cart"></i>
                  <strong class="badge">5</strong>
                </a>
  
                <button class="sm-hidden gnb-avatar-button" type="button" aria-label="마이메뉴 열기 버튼">
                  <div class="avatar-32">
                    <img src="./assets/images/img-user-01.jpg" alt="사딸라아저씨">
                  </div>
                </button>
              </div> 
              
```