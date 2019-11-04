---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 513ddffef8ac7a35133ca6bab402346d0c66b02d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936737"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = await graphClient.ConditionalAccess.Policies["{id}"]
    .Request()
    .GetAsync();

```