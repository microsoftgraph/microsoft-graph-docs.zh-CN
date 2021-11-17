---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 533d5775496f4b040f0bba283c445c867002941d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977783"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
displayName := "Library Assist"
requestBody.SetDisplayName(&displayName)
description := "Self help community for library"
requestBody.SetDescription(&description)
mailNickname := "libassist"
requestBody.SetMailNickname(&mailNickname)
partsToClone := "apps,tabs,settings,channels,members"
requestBody.SetPartsToClone(&partsToClone)
visibility := "public"
requestBody.SetVisibility(&visibility)
options := &msgraphsdk.CloneRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Clone().Post(options)


```