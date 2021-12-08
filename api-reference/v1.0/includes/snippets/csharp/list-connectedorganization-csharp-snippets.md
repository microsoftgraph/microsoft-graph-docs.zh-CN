---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a11c450ef139462392328150bdcd78f2bcac4515
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganizations = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations
    .Request()
    .GetAsync();

```