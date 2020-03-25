---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd61bb14a014065643998c5dd580011ccffb66a2
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947168"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("startswith(displayName,'Eric'),")
    .Select( e => new {
             e.DisplayName,
             e.SignInActivity 
             })
    .GetAsync();

```