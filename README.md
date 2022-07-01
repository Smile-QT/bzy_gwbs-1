## 构建镜像

- Dockerfile
- docker-compose.yml

```
# 生成镜像文件
docker-compose up --build

```

## 初始配置

- 1.应用数据库

```
python manage.py migrate
```

- 2.创建超级管理员

```
python namage.py createsuperuser
```

## 启动运行

```
# 后台运行
docker-compose up -d

# 前台地址
http://localhost:9000

# 后台地址
http://localhost:9000/admin/
```

## 注意事项

- 测试数据库使用SQLite
- 正式数据库使用MySQL, PostgreSQL
- 需要创建数据库