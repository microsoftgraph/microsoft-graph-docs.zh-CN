---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4db76d869bf1ab30aec3e442dd8d33b6e4e1a073
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335792"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyCrossTenantAccessPolicyPartner -CrossTenantAccessPolicyConfigurationPartnerTenantId $crossTenantAccessPolicyConfigurationPartnerTenantId

```