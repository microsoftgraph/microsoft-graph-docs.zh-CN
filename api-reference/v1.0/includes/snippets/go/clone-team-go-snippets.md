---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b42ce304a1218bcde27f1c0085a70de17c9fc470
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325715"
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
teamId := "team-id"
graphClient.TeamsById(&teamId).Clone(team-id).Post(requestBody)


```