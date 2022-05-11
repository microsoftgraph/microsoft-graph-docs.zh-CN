---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 922279a6ab8eeb83ab37b4c45f95800580cc6144
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328364"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAppRoleAssignment()
principalId := "7679d9a4-2323-44cd-b5c2-673ec88d8b12"
requestBody.SetPrincipalId(&principalId)
resourceId := "076e8b57-bac8-49d7-9396-e3449b685055"
requestBody.SetResourceId(&resourceId)
appRoleId := "00000000-0000-0000-0000-000000000000"
requestBody.SetAppRoleId(&appRoleId)
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AppRoleAssignments().Post(requestBody)


```