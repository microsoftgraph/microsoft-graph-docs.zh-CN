---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c3f556fcdd217eec2b47b0772c89ab2ab7ca2f0
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legalHolds = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].LegalHolds
    .Request()
    .GetAsync();

```