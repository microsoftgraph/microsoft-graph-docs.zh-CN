---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46c6baaf93ec81b553e01d807273ac87f9c7a9c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UnifiedGroupSources["{ediscovery.unifiedGroupSource-id}"]
    .Request()
    .DeleteAsync();

```