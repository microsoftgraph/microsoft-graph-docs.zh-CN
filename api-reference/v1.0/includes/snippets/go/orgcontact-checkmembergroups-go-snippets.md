---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc5ffbd63cac471e406398b377553868b5d30717
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081972"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetGroupIds( []String {
    "groupId-value1",
    "groupId-value2",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).CheckMemberGroups().Post(options)


```