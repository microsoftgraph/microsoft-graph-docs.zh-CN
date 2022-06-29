---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b42a7c0d4187c3f5a4c4e1998d9120d8b5f73bb
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66503000"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Ids = @(
        "fa8bf3dc-eca7-46b7-bad1-db199b62afc3"
        "66825e03-7ef5-42da-9069-724602c31f6b"
    )
}

Get-MgCommunicationPresenceByUserId -BodyParameter $params

```