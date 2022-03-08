---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06b2f633de605a31f8225089e1caf6ea082dc3c2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customAccessPackageWorkflowExtension = {
    displayName: 'test_action_0124', 
    description: 'this is for graph testing only', 
    endpointConfiguration: { 
        '@odata.type': '#microsoft.graph.logicAppTriggerEndpointConfiguration', 
        subscriptionId: '38ab2ccc-3747-4567-b36b-9478f5602f0d', 
        resourceGroupName: 'EMLogicApp', 
        logicAppWorkflowName: 'customextension_test' 
    }, 
    authenticationConfiguration: { 
        '@odata.type': '#microsoft.graph.azureAdTokenAuthentication', 
        resourceId: 'f604bd15-f785-4309-ad7c-6fad18ddb6cb' 
    } 
};

await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/32efb28c-9a7a-446c-986b-ca6528c6669d/customAccessPackageWorkflowExtensions')
    .version('beta')
    .post(customAccessPackageWorkflowExtension);

```