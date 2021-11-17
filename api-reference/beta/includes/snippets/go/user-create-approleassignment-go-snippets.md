---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bb40036a667f64c933d7ee51c67afc98f536c56
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031485"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAppRoleAssignment()
principalId := "cde330e5-2150-4c11-9c5b-14bfdc948c79"
requestBody.SetPrincipalId(&principalId)
resourceId := "8e881353-1735-45af-af21-ee1344582a4d"
requestBody.SetResourceId(&resourceId)
appRoleId := "00000000-0000-0000-0000-000000000000"
requestBody.SetAppRoleId(&appRoleId)
options := &msgraphsdk.AppRoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).AppRoleAssignments().Post(options)


```