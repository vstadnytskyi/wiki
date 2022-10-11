We want to set up automatic upload of new version of our repository on PyPi and TestPyPi. One great way to do it is GitHub actions. 

### Step 1 

Follow instructions here https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/

### Step 2: 
Create Secret Token in your repository
1. login to https://test.pypi.org
2. go to account settings /n <img width="216" alt="image" src="https://user-images.githubusercontent.com/29989124/194669701-e59b075c-8f4e-4ca5-8977-0ab0eb02f7f0.png">
3. scroll down until you find API Token
4. Add API token
5. Follow instructions

Copy the token and go to your GitHub profile 
add token as secret
<img width="363" alt="image" src="https://user-images.githubusercontent.com/29989124/194670084-d2191be8-ac1a-49e2-9499-c72afcc1ee9a.png">
in "Settings" -> "Secrets" -> "Actions" of the repository you are setting this up.

In my GitHub workflow examples I called the "PUSH_TO_TESTPYPI" and "PUSH_TO_PYPI".
See ciruclar buffer numpy for working examples. 
<img width="598" alt="image" src="https://user-images.githubusercontent.com/29989124/195217502-fc11f455-102f-4a38-843a-09fee67e3181.png">
