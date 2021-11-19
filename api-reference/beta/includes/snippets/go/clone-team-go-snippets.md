---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1eee042bb1185c4040ac82d4eb1d00ae56f62baa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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