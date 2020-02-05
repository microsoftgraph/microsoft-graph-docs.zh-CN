---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dec793cf699a1407ab51a89e6febdf74599639df
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41778015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.UserPrincipalName,
             e.SignInActivity 
             })
    .GetAsync();

```