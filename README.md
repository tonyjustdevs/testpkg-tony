# Tony's Example Package

[Tutorial Reference Link](https://packaging.python.org/en/latest/tutorials/packaging-projects/)

# Notes for self:
- or git clone ... or 
- or gh repo create testpkg-tony --public --source=. --push
- or pip install -e git+https://github.com/numpy/numpy.git@v1.25.0#egg=numpy
- or pip install -e git+https://github.com/owner/repo.git@branch#egg=package
- or pip install -e git+https://<TOKEN>@github.com/owner/repo.git@branch#egg=package_name 
- or pip install -e git+ssh://git@github.com/owner/repo.git@main#egg=private_pkg
- && cd ... && 
- pip install -e . or pip install -e ".[dev]"
- python -c "import my_package; print(my_package.__file__)"
- git commit -am "Prepare release v..."
- git tag -a v1.0.0 -m "Release v..."
- git push origin main --tags
- rm -rf dist
- pip install build twine 
- python -m build
- twine upload -r testpypi dist/*
- pip install dist/my_package-v0.0.0.whl
- python -c "import my_package; print(my_package.__file__)
- pip install -e .