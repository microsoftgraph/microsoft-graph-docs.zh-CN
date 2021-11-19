---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e32ecc8f81d46e9c24093fee1b895dd976b8265
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084509"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAppRoleAssignment()
principalId := "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
requestBody.SetPrincipalId(&principalId)
resourceId := "8fce32da-1246-437b-99cd-76d1d4677bd5"
requestBody.SetResourceId(&resourceId)
appRoleId := "498476ce-e0fe-48b0-b801-37ba7e2685c6"
requestBody.SetAppRoleId(&appRoleId)
options := &msgraphsdk.AppRoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignments().Post(options)


```