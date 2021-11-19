---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2baef4d8e106896f7d5461a4796f73600ceb042
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087679"
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
options := &msgraphsdk.AppRoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AppRoleAssignments().Post(options)


```