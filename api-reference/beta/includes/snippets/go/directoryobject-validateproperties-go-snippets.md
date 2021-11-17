---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4a1d8a652d1f9bb16417952b8172e29e44ded5d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015628"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
entityType := "Group"
requestBody.SetEntityType(&entityType)
displayName := "Myprefix_test_mysuffix"
requestBody.SetDisplayName(&displayName)
mailNickname := "Myprefix_test_mysuffix"
requestBody.SetMailNickname(&mailNickname)
onBehalfOfUserId := "onBehalfOfUserId-value"
requestBody.SetOnBehalfOfUserId(&onBehalfOfUserId)
options := &msgraphsdk.ValidatePropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.DirectoryObjects().ValidateProperties().Post(options)


```