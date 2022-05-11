---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10ec145245313fae1e9fd070adfd44d7d2857aec
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328680"
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
graphClient.DirectoryObjects().ValidateProperties().Post(requestBody)


```