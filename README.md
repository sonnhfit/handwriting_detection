# django-deap-learning-mnist-sample


```
git clone https://github.com/sonnhfit/handwriting_detection.git
```


cd vao thu muc vua clone veva tao env
```
cd handwriting_detection 
python -m venv env
env\Scripts\activate
# cai thu vien
pip install -r requirements.txt
```

```
python manage.py migrate
```



```
python manage.py runserver
```
Nếu chạy chỗ này bị lỗi thì chắc là do môi trường máy bạn bạn, mình chạy trên windows. Nếu bạn muốn chạy trên macos hoặc linux, ubuntu... thì vào phần sau đây sửa đường dẫn đến model:
File: `/mnist/views.py` Dòng số 10
`model_path = current_dir + '\\model\\mnist.h5'` sửa thành `model_path = current_dir + '/model/mnist.h5'` để chạy trên mac hoặc linux
```
http://localhost:8000/mnist
```


