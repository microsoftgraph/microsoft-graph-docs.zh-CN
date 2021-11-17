---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c097d242f951badaa3c4b2a15479a0e8117285d32cbc88973484a23b8a73475
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entitlementManagementSettings = await graphClient.IdentityGovernance.EntitlementManagement.Settings
    .Request()
    .GetAsync();

```