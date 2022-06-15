---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c3f0e7af86e378b5824624c9c639669736d645f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"].CustodianSources["{security.dataSource-id}"].Reference
    .Request()
    .DeleteAsync();

```