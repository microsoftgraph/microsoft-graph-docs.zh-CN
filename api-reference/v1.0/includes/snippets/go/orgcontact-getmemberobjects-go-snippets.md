---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 376a59333c1d24610942a682f88ad71b6e259957
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992815"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
securityEnabledOnly := false
requestBody.SetSecurityEnabledOnly(&securityEnabledOnly)
options := &msgraphsdk.GetMemberObjectsRequestBuilderPostOptions{
    Body: requestBody,
}
orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).GetMemberObjects().Post(options)


```