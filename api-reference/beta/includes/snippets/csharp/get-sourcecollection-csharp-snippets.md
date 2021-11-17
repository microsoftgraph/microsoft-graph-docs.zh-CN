---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4123b64bbd58e420183a9a027bd60938e57eecf5042c59b790a11295e45015d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceCollection = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .Request()
    .Expand("lastEstimateStatisticsOperation")
    .GetAsync();

```