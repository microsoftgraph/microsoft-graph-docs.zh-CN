---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c422a774c0f6a8814670a99f7324ba33db62ff2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .OrderBy("displayName ")
    .GetAsync();

```