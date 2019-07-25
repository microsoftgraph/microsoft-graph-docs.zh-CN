---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a62e4b948881ebf03ea520fc61598d09edb8764
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .Stop()
    .Request()
    .PostAsync();

```