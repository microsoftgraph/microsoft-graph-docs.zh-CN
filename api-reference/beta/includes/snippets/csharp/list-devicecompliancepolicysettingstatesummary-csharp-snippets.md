---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b05fd72647020ea30735de0afbc4c416df8d0da33eefbe63c20a459223f73579
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceCompliancePolicySettingStateSummary = await graphClient.TenantRelationships.ManagedTenants.DeviceCompliancePolicySettingStateSummary
    .Request()
    .GetAsync();

```