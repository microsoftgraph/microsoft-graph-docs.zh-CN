---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62a59c6df630ec4cb29d0e38d103d091f93aede2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329074"
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
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignedTo().Post(requestBody)


```