---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa4a601c1e9335fa36a6c0349f0d2d4dff3e852c
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```