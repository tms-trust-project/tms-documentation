=================
TMS Documentation
=================

readthedocs documentation for the TACC Trust Manager System (TMS)

Quickstart
----------
This repository contains the source of the documentation of TACC TMS project. You can build a local version
of this repository with Sphinx in a Python 3 environment (if you do not have Python
installed there are many good resources on the Internet to walk you through installation on your
operating system).

1. Install Sphinx using ``pip install sphinx``
2. Install the Read the Docs theme ``pip install sphinx-rtd-theme``
3. Fork the repository to your personal Github account.
4. Copy the repo from your account to your local system (using your favorite method: HTTPS, SSH, the Github CLI, or the Github Desktop app).
5. Navigate to the repo directory on your local system
6. Build the repo using ``make html`` (Mac/Linux) or ``make.bat html`` (Windows).
7. Open the file ``[name of local repo]/build/html/index.html`` in your browser.

Note that if you replace step 1 above with ``pip install sphinx-autobuild``, you can use
``make livehtml`` which will start a server that watches for source changes and will
rebuild/refresh automatically. Go to http://localhost:7898/ to see its output.

