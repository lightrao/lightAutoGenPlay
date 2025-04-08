% python3 -m venv .venvAutoGen    
% source /Users/developrao/Documents/LightTechZen/lightAutoGenPlay/.venvAutoGen/bin/activate (for powershell: .\.venvAutoGen\Scripts\Activate)
% uv pip install -U autogenstudio
% uv pip install PySocks
% uv pip install "httpx[socks]"
% uv pip freeze > requirements.txt

% autogenstudio ui --port 8081 --appdir ./myapp