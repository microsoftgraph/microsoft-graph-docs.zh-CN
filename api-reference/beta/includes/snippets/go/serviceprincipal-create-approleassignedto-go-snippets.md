---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54bdeb8f773f37976823b98fd29b9fb625576438
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093606"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAppRoleAssignment()
principalId := "33ad69f9-da99-4bed-acd0-3f24235cb296"
requestBody.SetPrincipalId(&principalId)
resourceId := "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
requestBody.SetResourceId(&resourceId)
appRoleId := "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
requestBody.SetAppRoleId(&appRoleId)
options := &msgraphsdk.AppRoleAssignedToRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignedTo().Post(options)


```