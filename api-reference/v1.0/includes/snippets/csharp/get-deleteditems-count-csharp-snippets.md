---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13193a01dcb322ddea05954fbbdb662a11ede963
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767264"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Directory.DeletedItems
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Select("id,displayName,deletedDateTime")
    .OrderBy("deletedDateTime asc")
    .GetAsync();

```