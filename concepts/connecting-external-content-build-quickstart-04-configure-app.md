---
ms.localizationpriority: medium
ms.openlocfilehash: e04c28e801be69487d83e5b5a3184c4702652aa3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289520"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

1. 在 PartsInventoryConnector.csproj 所在的 (CLI) 打开命令行接口。
2. 运行以下命令以初始化项目的用户密码。

    ```dotnetcli
    dotnet user-secrets init
    ```

3. 运行以下命令，将应用 ID、应用密码和租户 ID 存储在用户密码存储中。

    ```dotnetcli
      dotnet user-secrets set appId "YOUR_APP_ID_HERE"
      dotnet user-secrets set appSecret "YOUR_APP_SECRET_HERE"
      dotnet user-secrets set tenantId "YOUR_TENANT_ID_HERE"
    ```
