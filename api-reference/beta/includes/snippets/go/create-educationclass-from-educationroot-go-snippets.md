---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 014ea63502c83af12e2e243956b62949d3f16007
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327988"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationClass()
description := "Health Level 1"
requestBody.SetDescription(&description)
classCode := "Health 501"
requestBody.SetClassCode(&classCode)
displayName := "Health 1"
requestBody.SetDisplayName(&displayName)
externalId := "11019"
requestBody.SetExternalId(&externalId)
externalName := "Health Level 1"
requestBody.SetExternalName(&externalName)
externalSource := "sis"
requestBody.SetExternalSource(&externalSource)
mailNickname := "fineartschool.net"
requestBody.SetMailNickname(&mailNickname)
result, err := graphClient.Education().Classes().Post(requestBody)


```