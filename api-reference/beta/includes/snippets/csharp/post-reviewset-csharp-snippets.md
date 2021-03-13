---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20c332320f5f6ea8bf4eefe97e0467eb659eaeff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802013"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSet = new Microsoft.Graph.Ediscovery.ReviewSet
{
    DisplayName = "My Reviewset 3"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets
    .Request()
    .AddAsync(reviewSet);

```