---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6eacb05bf87dd4668b836a5143a31928037cd03
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338197"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "test_action_0124"
    Description = "this is for graph testing only"
    EndpointConfiguration = @{
        "@odata.type" = "#microsoft.graph.logicAppTriggerEndpointConfiguration"
        SubscriptionId = "38ab2ccc-3747-4567-b36b-9478f5602f0d"
        ResourceGroupName = "EMLogicApp"
        LogicAppWorkflowName = "customextension_test"
    }
    AuthenticationConfiguration = @{
        "@odata.type" = "#microsoft.graph.azureAdTokenAuthentication"
        ResourceId = "f604bd15-f785-4309-ad7c-6fad18ddb6cb"
    }
}

New-MgEntitlementManagementAccessPackageCatalogCustomAccessPackageWorkflowExtension -AccessPackageCatalogId $accessPackageCatalogId -BodyParameter $params

```