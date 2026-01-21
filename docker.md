دستور	معنی	کاربرد	کاربرد	کاربرد	
docker compose up -d	دستوری برای راه‌اندازی تمام سرویس‌های تعریف‌شده در فایل docker-compose.yml	راه‌اندازی چندین کانتینر به صورت همزمان	ایجاد شبکه، volumeها و dependencies بین سرویس‌ها	اجرای کل استک برنامه با یک دستور	دشd بزنی در بک گراند اجرا میشه یعنی ترمینالت آزاد میشه
docker compose build --no-cache	بدون کش 				
docker ps  	لیست کانتینرهای در حال اجرا				
docker ps -a					
docker logs -f embedding-service	لاگ های کانترنرت تو داکر				
docker compose down	بستن داکراگر داکرکامپوز داری				
docker stop <container_id>	بستن کانتینر ها دستی				
docker exec -it نام_کانتینر psql -U نام_کاربر -d نام_دیتابیس	PostgreSQLورود به دیتابیس 	بعدش میتونی \dt  بزنی ساختارجدول ببینی			
docker exec -it نام_کانتینر bash	 اجرای دستور جدید در کانتینر در حال اجرا				
docker run -it نام_ایمیج bash	اجرای کانتینر جدید از یک image (اگر کانتینر در حال اجرا نباشد)				
docker start نام_کانتینر	 شروع یک کانتینر متوقف شده				
docker stop نام_کانتینر					
docker rm -f نام_کانتینر	حذف اجباری کانتینر				
docker rmi python:3.11.6	حذف یک ایمیج				
docker container prune -f	پاک کردن کل کش و کانتینرها	docker volume prune -f و docker image prune -f هم داره			
docker compose up -d --build --force-recreate backend					
docker pull python :3.14.0	دانلود ایمیج پایتون 				
docker tag python:3.11.6 python-local:3.11.6	تگ میزنه به ایمیجت / اسم میزاره براش و بعنوان ایمیج محلی میشناسه				
docker run -it --rm alpine:latest sh	۱. تست سریع محیط Linux:۲. عیب‌یابی (Troubleshooting):	این دستور مثل باز کردن یک ترمینال لینوکس موقتی و پاکشونده است - عالی برای آزمایش و یادگیری!			
