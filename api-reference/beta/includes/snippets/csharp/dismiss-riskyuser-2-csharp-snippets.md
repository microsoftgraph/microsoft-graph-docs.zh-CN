---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91d32f32c51b4cb9c63f6f05e16f8cc94ee09391
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "04487ee0-f4f6-4e7f-8999-facc5a30e232"
};

await graphClient.IdentityProtection.RiskyUsers
    .Dismiss(userIds)
    .Request()
    .PostAsync();

```