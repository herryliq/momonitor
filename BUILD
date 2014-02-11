from glob import glob

python_binary(
  name = 'momonitor',
  source = 'manage.py',
  dependencies = [
    pants(':momonitor_lib')
  ]
)

python_library(
  name = 'momonitor_lib',
  sources = rglobs('*.py') - ['manage.py'],
  resources = rglobs('common/static/*', 'common/templates/*'),
  dependencies = [
    python_requirement('Django==1.4.3'),
    python_requirement('Flask==0.9'),
    python_requirement('Jinja2==2.6'),
    python_requirement('Pygments==1.6'),
    python_requirement('South==0.7.6'),
    python_requirement('Sphinx==1.1.3'),
    python_requirement('Werkzeug==0.8.3'),
    python_requirement('croniter==0.3.3'),
    python_requirement('django-breadcrumbs==1.1.3-p1'),
    python_requirement('django-redis==3.1.6'),
    python_requirement('django-social-auth==0.7.18'),
    python_requirement('django-tastypie==0.9.14'),
    python_requirement('docutils==0.10'),
    python_requirement('gevent==0.13.8'),
    python_requirement('greenlet==0.4.0'),
    python_requirement('httplib2==0.8'),
    python_requirement('mimeparse==0.1.3'),
    python_requirement('oauth2==1.5.211'),
    python_requirement('psycopg2==2.4.6'),
    python_requirement('python-dateutil==1.5'),
    python_requirement('python-openid==2.2.5'),
    python_requirement('redis==2.7.2'),
    python_requirement('requests==1.1.0'),
    python_requirement('six==1.3.0'),
    python_requirement('wsgiref==0.1.2'),
    #python_requirement('zope.interface==4.0.3'),
  ]
)
