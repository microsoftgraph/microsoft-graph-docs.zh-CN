---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 652f4ac3466b84249c4db863fd2f2743b7f3176b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325798"
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
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignments().Post(requestBody)


```