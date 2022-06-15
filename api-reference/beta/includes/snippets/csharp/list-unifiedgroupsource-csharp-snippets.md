---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ab4a8c5a3b9be1df12b5c801191a9353e620238
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094960"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSources = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"].UnifiedGroupSources
    .Request()
    .GetAsync();

```