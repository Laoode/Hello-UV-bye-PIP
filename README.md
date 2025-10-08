# Uv is 100x faster than pip because it's written in Rust

How to install uv
bash'''
pip install uv
'''

Check uv has been installed
bash'''
uv
'''

Check our python version
bash'''
uv python list
'''

If we want to install a particular python installation 
bash'''
uv python install 3.12
'''

Search particular version
bash'''
uv python find 3.12
'''

For uninstall the python version
bash'''
uv python uninstall 3.12
'''

Running python script
bash'''
uv run main.py
'''

If we want to use specify of python version when we're running particular script
bash'''
uv run --python 3.9.21 main.py
'''

Run python script with the dependency hasn't installed yet
bash'''
# import rich
# import requests
uv run --with rich --with requests --python 3.9.12 main.py
'''

Create project with uv
bash'''
uv init
'''

Add dependency
bash'''
uv add requests
'''

Remove dependency
bash'''
uv remove requests
'''