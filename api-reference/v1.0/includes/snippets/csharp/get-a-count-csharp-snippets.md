---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34c1977bcdd4930ae245f7817e9461d551b5cd0c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName,'a'),")
    .OrderBy("displayName ")
    .Top(1)
    .GetAsync();

```