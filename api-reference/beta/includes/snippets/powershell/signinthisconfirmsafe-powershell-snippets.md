---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 788708b311894a1cf54287658b094adacad152cc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447240"
---
```powershell

Import-Module Microsoft.Graph.Reports

$params = @{
    RequestIds = @(
        "5a0c76d2-cb57-4ece-9bc1-c323178f116a"
        "96609214-09ef-4f80-9d4a-ace5fceecaec"
        "05020696-4eb8-45a3-918f-8f8bb7ad6015"
    )
}

Confirm-MgAuditLogSignInSafe -BodyParameter $params

```