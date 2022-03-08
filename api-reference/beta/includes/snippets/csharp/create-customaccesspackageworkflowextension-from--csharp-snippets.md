---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3a225115d5d3c7f2e085f24a1b057bc08ecab00
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customAccessPackageWorkflowExtension = new CustomAccessPackageWorkflowExtension
{
    DisplayName = "test_action_0124",
    Description = "this is for graph testing only",
    EndpointConfiguration = new LogicAppTriggerEndpointConfiguration
    {
        SubscriptionId = "38ab2ccc-3747-4567-b36b-9478f5602f0d",
        ResourceGroupName = "EMLogicApp",
        LogicAppWorkflowName = "customextension_test"
    },
    AuthenticationConfiguration = new AzureAdTokenAuthentication
    {
        ResourceId = "f604bd15-f785-4309-ad7c-6fad18ddb6cb"
    }
};

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"].CustomAccessPackageWorkflowExtensions
    .Request()
    .AddAsync(customAccessPackageWorkflowExtension);

```