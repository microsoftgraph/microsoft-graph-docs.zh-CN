---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34c1977bcdd4930ae245f7817e9461d551b5cd0c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335790"
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