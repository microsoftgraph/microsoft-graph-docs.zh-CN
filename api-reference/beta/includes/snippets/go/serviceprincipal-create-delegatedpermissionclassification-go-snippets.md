---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb68cf224d2e8814c61d3a4ffa1acba504d90646
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088749"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDelegatedPermissionClassification()
permissionId := "e1fe6dd8-ba31-4d61-89e7-88639da4683d"
requestBody.SetPermissionId(&permissionId)
permissionName := "User.Read"
requestBody.SetPermissionName(&permissionName)
classification := "low"
requestBody.SetClassification(&classification)
options := &msgraphsdk.DelegatedPermissionClassificationsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).DelegatedPermissionClassifications().Post(options)


```