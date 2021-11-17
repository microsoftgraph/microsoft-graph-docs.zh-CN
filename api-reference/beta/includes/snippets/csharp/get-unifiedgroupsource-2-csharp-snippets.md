---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47a398ef6859de96b1393958019f7fc32d0d1d73729e3ecc8e2a6a0a1f1057b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218565"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UnifiedGroupSources["{ediscovery.unifiedGroupSource-id}"]
    .Request()
    .GetAsync();

```