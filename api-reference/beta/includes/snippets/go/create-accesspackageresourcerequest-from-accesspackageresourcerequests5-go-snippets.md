---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d454ca116f2a6e7e0528ac99035e37b83cd2474c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119059"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "beedadfe-01d5-4025-910b-84abb9369997"
requestBody.SetCatalogId(&catalogId)
requestType := "AdminRemove"
requestBody.SetRequestType(&requestType)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
id := "354078e5-dbce-4894-8af4-0ab274d41662"
accessPackageResource.SetId(&id)
options := &msgraphsdk.AccessPackageResourceRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(options)


```