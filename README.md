# [Django Admin Berry](https://appseed.us/product/berry-dashboard/django/)

Modern template for **Django Admin Interface** coded on top of **[Berry Dashboard](https://appseed.us/product/berry-dashboard/django/)**, an open-source `Boostrap 5` design from `CodedThemes`. It is designed to deliver the best possible user experience with highly customizable feature-rich pages. `Berry` has easy and intuitive responsive design whether it is viewed on retina screens or laptops.

> Actively supported by [AppSeed](https://appseed.us/) via `Email` and `Discord`.

<br>

## Links & `Resources`

- [Django Berry](https://appseed.us/product/berry-dashboard/django/) - `Product page`
  - `Features`: Fully-configured, `CI/CD` via Render
- **UI Kit**: [Berry Bootstrap](https://codedthemes.com/item/berry-bootstrap-free-admin-template/?ref=appseed) by `CodedThemes`
- **Sections Covered**: 
  - `Admin Section`, reserved for `superusers`
  - `All pages` managed by `Django.contrib.AUTH`
  - `Registration` page
  - `Misc pages`: colors, icons, typography, blank-page 

<br />

![Berry Bootstrap 5 - Dark-Mode ready, Open-source Template.](https://user-images.githubusercontent.com/51070104/207091062-e805b36c-663a-4a01-acb8-9c55ab914f4f.jpg)

<br />

## Why `Django Admin Berry`

- Modern [Bootstrap 5](https://www.admin-dashboards.com/bootstrap-5-templates/) Design
- `Responsive Interface`
- `Minimal Template` overriding
- `Easy integration`

Berry Dashboard comes with error/bug-free, well structured codebase that renders nicely in all major browsers and devices. 

<br />

## How to use it

<br />

> **Install the package** via `PIP` 

```bash
$ pip install django-admin-berry
// OR
$ pip install git+https://github.com/app-generator/django-admin-berry.git
```

<br />

> Add `admin_berry` application to the `INSTALLED_APPS` setting of your Django project `settings.py` file (note it should be before `django.contrib.admin`):

```python
    INSTALLED_APPS = (
        ...
        'admin_berry.apps.AdminBerryConfig',
        'django.contrib.admin',
    )
```

<br />

> Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:

```python
    LOGIN_REDIRECT_URL = '/'
    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
```

<br />

> Add `admin_berry` urls in your Django Project `urls.py` file

```python
    from django.urls import path, include

    urlpatterns = [
        ...
        path('', include('admin_berry.urls')),
    ]
```

<br />

> **Collect static** if you are in `production environment`:

```bash
$ python manage.py collectstatic
```

<br />

> **Start the app**

```bash
$ # Set up the database
$ python manage.py makemigrations
$ python manage.py migrate
$
$ # Create the superuser
$ python manage.py createsuperuser
$
$ # Start the application (development mode)
$ python manage.py runserver # default port 8000
```

Access the `admin` section in the browser: `http://127.0.0.1:8000/`

<br />

## [PRO Version](https://appseed.us/product/berry-dashboard-pro/django/)   

This design is a pixel-perfect [Bootstrap 5](https://www.admin-dashboards.com/bootstrap-5-templates/) Dashboard with a fresh, new design inspired by Google's Material Design. `Material Dashboard 2 PRO` is built with over 300 frontend individual elements, like buttons, inputs, navbars, nav tabs, cards, or alerts, giving you the freedom of choosing and combining.

> Features: 

- `Up-to-date Dependencies`
- `Design`: [Django Theme Berry](https://github.com/app-generator/django-admin-berry-pro) - `PRO Version`
- `Sections` covered by the design:
  - **Admin section** (reserved for superusers)
  - **Authentication**: `Django.contrib.AUTH`, Registration
  - **All Pages** available in for ordinary users 
- `Docker`, `Deployment`:
  - `CI/CD` flow via `Render`

<br />

![Berry Bootstrap 5 PRO - Premium Template Django Template.](https://user-images.githubusercontent.com/51070104/210833058-be0b3e87-4f2b-4765-b84d-3795ba03c6a1.jpg)

<br />

---
**[Django Admin Berry](https://appseed.us/product/berry-dashboard/django/)** - Modern Admin Interface provided by **[AppSeed](https://appseed.us/)**
