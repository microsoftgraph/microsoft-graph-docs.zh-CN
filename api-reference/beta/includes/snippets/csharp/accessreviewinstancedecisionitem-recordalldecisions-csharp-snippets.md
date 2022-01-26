---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba6614d54ce4550b869dc146592fab095e686f94
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decision = "Deny";

var justification = "Alice switched teams and no longer works with this group";

var principalId = "2043848d-e422-473c-8607-88a3319ff491";

var resourceId = "733ef921-89e1-4d7e-aeff-83612223c37e";

await graphClient.IdentityGovernance.AccessReviews.Decisions
    .FilterByCurrentUser(null)
    .RecordAllDecisions(decision,justification,principalId,resourceId)
    .Request()
    .PostAsync();

```