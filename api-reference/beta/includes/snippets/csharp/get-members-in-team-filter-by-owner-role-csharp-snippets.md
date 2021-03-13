---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67da28dda7382a011656f9e4d2fbb5de0464727d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810243"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["{team-id}"].Members
    .Request()
    .Filter("roles/any(r:r eq 'owner')")
    .GetAsync();

```