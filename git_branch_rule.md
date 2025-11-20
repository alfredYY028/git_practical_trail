graph LR
    A[仓库] --> B(分支保护规则)
    B --> C{设置条件}
    C -->|Required reviews| D[指定审核人]
    C -->|Require status checks| E[CI验证]
    C -->|Restrict pushes| F[指定推送者]