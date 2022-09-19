# Gimmunity
- 기숙사생들의 활발한 소통을 위한 커뮤니티
- 수민외3(공도윤, 김수민, 전유리, 홍해인)
- 미림 스타트업 창업발표회 대상 수상작
- [기획서](https://bit.ly/3Tq5i80)
  - 미림 계정 로그인, 기숙사생 전용 질문을 통과해야 가입 가능
  - 게시물 조회
  - 게시물 추가
  - 댓글
  - 기숙사 공지사항, 생활 규칙 전달
---
1. startproject
   1. python -m pip install django~=3.2
   2. django-admin startproject Gimmunity .
   3. python manage.py runserver
2. startapp notice
   1. python manage.py startapp notice
   2. 'notice', in INSTALLED_APPS in settings.py
   3. models -> admin -> views -> templates -> urls
   4. models
      1. Notice
      2. python manage.py makemigrations notice
      3. python manage.py migrate notice
   5. admin
      1. NoticeAdmin
      2. python manage.py createsuperuser
   6. views
      1. NoticeListView
      2. NoticeDetailView
   7. templates
      1. notice_list.html
      2. notice_detail.html
   8. urls
      1. notice:list
      2. notice:detail
3. startapp post
   1. python manage.py startapp post
   2. 'post', in INSTALLED_APPS in settings.py
   3. models
      1. Post
      2. Comment
      3. python manage.py makemigrations post
      4. python manage.py migrate post
   4. admin
   5. views
   6. templates
   7. urls