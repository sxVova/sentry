# Playbook for *DEMO3*

This **playbooks** can automatically deploy the necessary *infrastructure*.  
**Flask role** pulls the application *image* onto the machine and launches it.  
**Sentry deploy role** sets *Sentry* and creates a *superuser*.  
For correct work of **sentry playbook** when building the image, you need to delete [27-38] lines from the   **src/sentry/receivers/users.py** file.  
**Sentry monitoring role** installs monitoring agent and enable the status information handlers in Nginx and memcached. The **role** also adds the *keys* of the required **IAM user**.
