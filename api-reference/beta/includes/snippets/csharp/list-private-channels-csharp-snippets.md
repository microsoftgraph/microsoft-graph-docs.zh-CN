---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4178a1c7cce23bca0862d0de29f98c62bd9a8a79
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402326"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channels = await graphClient.Teams["{id}"].Channels
    .Request()
    .Filter("membershipType eq 'private'")
    .GetAsync();

```