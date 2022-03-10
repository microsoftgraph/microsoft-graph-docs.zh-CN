---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae6ba52a40abcbcf57f58a40f82cd1a8dc7b7ecc
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411934"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
displayName := "Myprefix_test_mysuffix"
requestBody.SetDisplayName(&displayName)
mailNickname := "Myprefix_test_mysuffix"
requestBody.SetMailNickname(&mailNickname)
onBehalfOfUserId := "onBehalfOfUserId-value"
requestBody.SetOnBehalfOfUserId(&onBehalfOfUserId)
options := &msgraphsdk.ValidatePropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).ValidateProperties(group-id).Post(options)


```