---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65c3bca0050be6fbcff2aa0d54a12538f662952e7b13e2745196b67988ed1372
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedGroupSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Custodians["{ediscovery.custodian-id}"].UnifiedGroupSources
    .Request()
    .GetAsync();

```