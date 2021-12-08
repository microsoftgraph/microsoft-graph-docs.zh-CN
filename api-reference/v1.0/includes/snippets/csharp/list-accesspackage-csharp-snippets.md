---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a5e30f02e355e129e17806da317987f18d4679f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackages = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .Request()
    .GetAsync();

```