---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baabcbbdfbf03b3bdce875f29e7bb0c993496eb6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Users.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```