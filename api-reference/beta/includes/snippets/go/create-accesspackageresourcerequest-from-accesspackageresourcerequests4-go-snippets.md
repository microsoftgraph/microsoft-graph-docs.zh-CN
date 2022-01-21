---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4edf2f37be6938a8fc7fda58a7a373cc3b69aff7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119060"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "beedadfe-01d5-4025-910b-84abb9369997"
requestBody.SetCatalogId(&catalogId)
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
originId := "c6294667-7348-4f5a-be73-9d2c65f574f3"
accessPackageResource.SetOriginId(&originId)
originSystem := "AadGroup"
accessPackageResource.SetOriginSystem(&originSystem)
options := &msgraphsdk.AccessPackageResourceRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(options)


```