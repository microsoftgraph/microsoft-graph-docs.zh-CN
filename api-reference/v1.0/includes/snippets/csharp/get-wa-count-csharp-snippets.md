---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08bcb82b64c605474cf75b3f77b9e59011cc4d9d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .OrderBy("displayName")
    .GetAsync();

```