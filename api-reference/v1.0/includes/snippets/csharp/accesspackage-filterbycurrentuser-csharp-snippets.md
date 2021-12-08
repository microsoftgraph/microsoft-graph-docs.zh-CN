---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67db238aeb820c336056e662732f6e49b6685b37
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .FilterByCurrentUser(AccessPackageFilterByCurrentUserOptions.AllowedRequestor)
    .Request()
    .GetAsync();

```