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
    "files.trimTrailingWhitespace": true,
    "workbench.startupEditor": "none"
}
```
### Visual Studio 2022 があるなら最新に更新、なければ以下

[![image](https://user-images.githubusercontent.com/1501327/184050608-6b5c686f-324c-41cb-bd1d-4cd227003e58.png)](https://dotnet.microsoft.com/ja-jp/download/dotnet/6.0)

![image](https://user-images.githubusercontent.com/1501327/183581334-1f7641c8-fdb8-433f-9729-7c6e094740e1.png)

### 拡張
![image](https://user-images.githubusercontent.com/1501327/183583332-de4df410-9f25-4eb8-8aec-6a62e2d75bef.png)

### 実行
- F1 > workbench.action.closeFolder で全て閉じる
- form_01 フォルダをドラッグ&ドロップ
- setup.bat
- run.bat
- Form1.cs を選択して表示( **Yes を選択** )\
    ![image](https://user-images.githubusercontent.com/1501327/184465924-057b000d-e524-4732-ae21-5abd5869f5b1.png)

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
        /* {
            "name": ".NET Core Attach",
            "type": "coreclr",
            "request": "attach"
        } */
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

### デバッグ
- アクティビティバーのデバッグアイコンでデバッグ用サイドバーを開く
- 左上、緑の右向き ▶ で実行\
    ![image](https://user-images.githubusercontent.com/1501327/184466220-c2a9d66a-4ffd-42a1-b67e-64c3f3d25668.png)





