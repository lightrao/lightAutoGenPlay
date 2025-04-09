% python3 -m venv .venvAutoGen    
% source /Users/developrao/Documents/LightTechZen/lightAutoGenPlay/.venvAutoGen/bin/activate 
for powershell: > .\.venvAutoGen\Scripts\Activate

% uv pip install autogenstudio
or
% python -m ensurepip --upgrade
% python -m pip install -U autogenstudio
% python -m pip list
% python.exe -m pip install --upgrade pip

% uv pip install PySocks
% uv pip install "httpx[socks]"
for powershel: > pip install openai
% uv pip freeze > requirements.txt

% autogenstudio ui --port 8081 --appdir ./myapp