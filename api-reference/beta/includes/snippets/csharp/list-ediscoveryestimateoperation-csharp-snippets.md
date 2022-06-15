---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d22254be6ac393d89094882ccfa86f8fc15e678
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryEstimateOperation = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"].LastEstimateStatisticsOperation
    .Request()
    .GetAsync();

```