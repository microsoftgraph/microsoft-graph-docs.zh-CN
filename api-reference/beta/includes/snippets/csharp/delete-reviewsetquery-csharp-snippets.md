---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5ad0e47954f04c182ec07f921f423d76da9c39c
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["2eef613a-ca2d-42f4-89fe-84d5198ddedf"].ReviewSets["b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8"].Queries["6b5358b0-2ce2-4369-b9cf-65392fe56807"]
    .Request()
    .DeleteAsync();

```