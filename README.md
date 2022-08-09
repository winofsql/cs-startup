# cs-startup

### settings.json
```json
{
    "-files.encoding": "shiftjis",
    "editor.mouseWheelZoom": true,
    "editor.fontSize": 16,
    "editor.renderWhitespace": "all",
    "terminal.integrated.fontSize": 16,
    "terminal.integrated.profiles.windows": {
        "Command Prompt": {
            "path": [
                "C:\\WINDOWS\\system32\\cmd.exe"
            ],
            "args": [],
            "icon": "terminal-cmd"
        }
    },
    "terminal.integrated.defaultProfile.windows": "Command Prompt",
    "window.zoomLevel": 1,
    "files.autoSave": "afterDelay",
    "workbench.startupEditor": "none"
}
```

![image](https://user-images.githubusercontent.com/1501327/183580326-0fb67b65-1ad0-463b-a087-0e74461cc320.png)

![image](https://user-images.githubusercontent.com/1501327/183581115-9d370144-b050-4e7f-b4b3-5f988fec2ac3.png)

![image](https://user-images.githubusercontent.com/1501327/183581334-1f7641c8-fdb8-433f-9729-7c6e094740e1.png)

![image](https://user-images.githubusercontent.com/1501327/183581797-c097a6cc-a4e4-4675-b593-936e8770cb39.png)

![image](https://user-images.githubusercontent.com/1501327/183582389-3e584a3c-63f2-4074-b9c8-d89c3e55877f.png)

![image](https://user-images.githubusercontent.com/1501327/183582477-9a330924-cdde-4c42-aa8e-bcc0c822bc3c.png)

![image](https://user-images.githubusercontent.com/1501327/183583332-de4df410-9f25-4eb8-8aec-6a62e2d75bef.png)

![image](https://user-images.githubusercontent.com/1501327/183583439-73e60dbb-e3d0-443d-9636-18db69dab756.png)

![image](https://user-images.githubusercontent.com/1501327/183583549-22efe106-b287-411b-a95f-9cae7107f0f0.png)

![image](https://user-images.githubusercontent.com/1501327/183584622-a30b12cc-f6dd-46eb-82b5-709721d36857.png)

![image](https://user-images.githubusercontent.com/1501327/183584747-68762fb5-3e10-44c4-b058-a23325721cc8.png)

### launch.json
```json
{
    // IntelliSense を使用して利用可能な属性を学べます。
    // 既存の属性の説明をホバーして表示します。
    // 詳細情報は次を確認してください: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": ".NET Core Launch (console)",
            "type": "coreclr",
            "request": "launch",
            "preLaunchTask": "build",
            "program": "${workspaceFolder}/cs_form_01/bin/Debug/net6.0-windows/cs_form_01.dll",
            "args": [],
            "cwd": "${workspaceFolder}/cs_form_01",
            // "console": "internalConsole",
            "console": "integratedTerminal",
            "stopAtEntry": false
        },
        {
            "name": ".NET Core Attach",
            "type": "coreclr",
            "request": "attach"
        }
    ]
}
```

### tasks.json
```jsom
{
    "version": "2.0.0",
    "tasks": [
        {
            "label": "build",
            "command": "dotnet",
            "type": "process",
            "args": [
                "build",
                "${workspaceFolder}/cs_form_01/cs_form_01.csproj",
                "/property:GenerateFullPaths=true",
                "/consoleloggerparameters:NoSummary"
            ],
            "problemMatcher": "$msCompile"
        },
        {
            "label": "publish",
            "command": "dotnet",
            "type": "process",
            "args": [
                "publish",
                "${workspaceFolder}/cs_form_01/cs_form_01.csproj",
                "/property:GenerateFullPaths=true",
                "/consoleloggerparameters:NoSummary"
            ],
            "problemMatcher": "$msCompile"
        },
        {
            "label": "watch",
            "command": "dotnet",
            "type": "process",
            "args": [
                "watch",
                "run",
                "--project",
                "${workspaceFolder}/cs_form_01/cs_form_01.csproj"
            ],
            "problemMatcher": "$msCompile"
        }
    ]
}
```
![image](https://user-images.githubusercontent.com/1501327/183586524-d3c0f756-256d-4f2e-af13-7271e785fc6a.png)

![image](https://user-images.githubusercontent.com/1501327/183585718-1a499b8f-ffd0-4426-be96-0b0c08e32844.png)

![image](https://user-images.githubusercontent.com/1501327/183585917-b504808c-bf6d-4150-a3f4-2a1304404808.png


### デバッガ無しで F5 で実行

![image](https://user-images.githubusercontent.com/1501327/183588718-696f6329-f6f5-4fad-a9fa-e4e6f59f0c6b.png)






