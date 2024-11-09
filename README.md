# hackathon-project

# Co-Art (다함께 그려요)

- Our website showcases a unique art experience where a new image is featured daily.
- Each image is converted into a pixelated canvas, allowing viewers to add on and modified the art.
- A carefully curated color palette accompanies each pixelated artwork, matching the image's original tones and adding an interactive, dynamic feel.
- After 24 hours, the artwork is moved to the gallery, where users can revisit and explore past creations.
- This evolving collection brings fresh visuals every day, blending technology and creativity in a digital gallery experience.

# 설명
 기술과 창의성은 조화를 이룹니다, 예술도 마찬가지입니다. 저희 조는 픽셀 브러쉬로 명화를 재현하고 덧그립니다. 사용자들은 명화의 한 부분을 구성하는 것으로 명작의 탄생에 직접 관여할 수 있습니다. 공동 작업을 통해 적은 노력으로 빠르게 작품을 완성시킬 수 있고, 그림의 색조와 유사한 팔레트가 제공됨으로써 미술적 감각을 기를 수 있습니다.
 매일 자정마다 최대 300x300픽셀이 비어 있는 이미지가 주어집니다. 사용자들은 이미지의 빈 공간에 픽셀 브러쉬와 다양한 색깔의 팔레트로 작품을 완성합니다. 우리 팀은 한 사람이 이미지의 너무 많은 부분을 점유하는 것을 피하기 위해 픽셀 브러쉬로 캔버스를 칠하는  시간 간격을 주었습니다. 또한 일부 사용자들의 고의적인 작품 방해를 막기 위해 픽셀 브러쉬로 칠할 수 있는 색상을 8가지로 제한하였습니다.  24시간 이후 이미지는 갤러리 구역으로 이동해 자유롭게 감상하거나, 다운로드 받을 수 있습니다.  Co-Art는 독특한 관객 참여형 예술 경험을 제공합니다.
 

# Backend Database

- Login
- Register
- UserProfile - including the time limit
- (daily) color palette
- Original art
- InProgress Pixel
- Completed Art

# Prerequisites

Instructions for Frontend

Install node from the website

> https://nodejs.org/en

Check the node version

> node -v

Locate the file and go into it

> cd C:\correct_path\Messenger-app

Install the necessary dependencie

> npm install

Run the dev mode server

> npm run dev

Click on the link

Instructions for Backend

imported

- Django
- channels
- websockets
- channels_redis
- djangorestframework
- django-cors-headers
- daphne

Download Python

> [Go to the official Python website.](https://www.python.org/downloads/)

- Run the downloaded installer.
  > check the box that says "Add Python to PATH"

Check python and pip version

> python --version
> pip --version

Install packages

> pip install django channels djangorestframework django-cors-headers channels_redis daphne

run server (init)

> python manage.py migrate

> python manage.py runserver

run docker for websockets (localhost for now)

> docker run -p 6379:6379 -d redis:5

create admin

> python manage.py createsuperuser

models to db migration

> python manage.py makemigrations

