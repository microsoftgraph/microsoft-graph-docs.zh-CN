---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f5acb2b9d7a3f30e9b0b5762bfd5c9580627702
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
};

await graphClient.IdentityProtection.RiskyUsers
    .Dismiss(userIds)
    .Request()
    .PostAsync();

```