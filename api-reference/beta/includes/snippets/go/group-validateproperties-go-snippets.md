---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3279777b833d8bb28023ec3d66be1cc5c642f6aa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327705"
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
groupId := "group-id"
graphClient.GroupsById(&groupId).ValidateProperties(group-id).Post(requestBody)


```