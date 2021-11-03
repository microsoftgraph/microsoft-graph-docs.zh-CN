---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6de2117ae32e99cd2f8ace4abb9b5bdea15e625309ae780e702839ea2c8b879
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903694"
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