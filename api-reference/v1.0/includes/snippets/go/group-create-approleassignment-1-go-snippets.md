---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04c44f6f9a2ff4b55d7c31100255fff3e1acfe46
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025281"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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