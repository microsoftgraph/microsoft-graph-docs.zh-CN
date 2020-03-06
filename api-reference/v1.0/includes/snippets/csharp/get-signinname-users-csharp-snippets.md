---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eca32b1aa75a09c03d3803a8f325ffe3c9594543
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')")
    .Select( e => new {
             e.DisplayName,
             e.Id 
             })
    .GetAsync();

```