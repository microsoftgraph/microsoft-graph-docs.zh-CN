---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 608739f8d8d7ac7ce7f617d199696c16b842d562
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325797"
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
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).DelegatedPermissionClassifications().Post(requestBody)


```