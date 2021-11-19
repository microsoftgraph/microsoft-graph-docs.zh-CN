---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57b4a0aaeb34a4b2c497401cbf4f295a92c7c0af
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083119"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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