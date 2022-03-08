---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cbcb8f4ec871813c5913e86466dbcac1d4927c2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338273"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.customAccessPackageWorkflowExtension",
    "displayName": "test_action_0124_email",
    "description": "this is for graph testing only",
}
options := &msgraphsdk.CustomAccessPackageWorkflowExtensionRequestBuilderPutOptions{
    Body: requestBody,
}
accessPackageCatalogId := "accessPackageCatalog-id"
customAccessPackageWorkflowExtensionId := "customAccessPackageWorkflowExtension-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).CustomAccessPackageWorkflowExtensionsById(&customAccessPackageWorkflowExtensionId).Put(options)


```