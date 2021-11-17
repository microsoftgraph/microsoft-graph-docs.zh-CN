---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82996f3eff7fe21ed7ed67f7791c681b86bd17ac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032220"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetGroupIds( []String {
    "groupIds-value",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).CheckMemberGroups().Post(options)


```