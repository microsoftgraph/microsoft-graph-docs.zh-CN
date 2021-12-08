---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ca70c415c3bb6dfa9a4edee23d08cea285a86f8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340079"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entitlementManagementSettings = await graphClient.IdentityGovernance.EntitlementManagement.Settings
    .Request()
    .GetAsync();

```