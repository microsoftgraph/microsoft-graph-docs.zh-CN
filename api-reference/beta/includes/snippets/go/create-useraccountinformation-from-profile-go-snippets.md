---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88c323c1022a6c35c0fb8b20636a9a5695890ba6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325844"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserAccountInformation()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
countryCode := "NO"
requestBody.SetCountryCode(&countryCode)
result, err := graphClient.Me().Profile().Account().Post(requestBody)


```