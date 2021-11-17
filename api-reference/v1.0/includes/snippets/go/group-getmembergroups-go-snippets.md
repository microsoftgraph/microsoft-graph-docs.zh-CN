---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cf4a8846c6b1bfa84af5d11d4823973c14afc7f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976698"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
securityEnabledOnly := false
requestBody.SetSecurityEnabledOnly(&securityEnabledOnly)
options := &msgraphsdk.GetMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).GetMemberGroups().Post(options)


```