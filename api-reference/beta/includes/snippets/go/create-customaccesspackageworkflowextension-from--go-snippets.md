---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75fa196626b259963f2ed15fa781f5be668153bc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326194"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustomAccessPackageWorkflowExtension()
displayName := "test_action_0124"
requestBody.SetDisplayName(&displayName)
description := "this is for graph testing only"
requestBody.SetDescription(&description)
endpointConfiguration := msgraphsdk.NewCustomExtensionEndpointConfiguration()
requestBody.SetEndpointConfiguration(endpointConfiguration)
endpointConfiguration.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.logicAppTriggerEndpointConfiguration",
    "subscriptionId": "38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "resourceGroupName": "EMLogicApp",
    "logicAppWorkflowName": "customextension_test",
}
authenticationConfiguration := msgraphsdk.NewCustomExtensionAuthenticationConfiguration()
requestBody.SetAuthenticationConfiguration(authenticationConfiguration)
authenticationConfiguration.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.azureAdTokenAuthentication",
    "resourceId": "f604bd15-f785-4309-ad7c-6fad18ddb6cb",
}
accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).CustomAccessPackageWorkflowExtensions().Post(requestBody)


```