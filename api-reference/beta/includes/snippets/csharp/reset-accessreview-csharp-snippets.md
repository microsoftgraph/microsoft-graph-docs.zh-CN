---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b7877ea77f412edbea4ec16e8bf631caa167455a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["2975E9B5-44CE-4E71-93D3-30F03B5AA992"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```