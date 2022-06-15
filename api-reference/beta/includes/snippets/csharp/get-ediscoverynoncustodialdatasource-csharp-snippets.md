---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ea42d35fc6b597b2745dd1247b046e587aab0d5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryNoncustodialDataSource = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].NoncustodialDataSources["{security.ediscoveryNoncustodialDataSource-id}"]
    .Request()
    .Expand("dataSource")
    .GetAsync();

```