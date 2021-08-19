---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8332ae258e14486175efe119362bd4879871f4d3bed85e8c9d785b67bb9b2a37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("endswith(mail,'a@contoso.com')")
    .OrderBy("userPrincipalName")
    .GetAsync();

```