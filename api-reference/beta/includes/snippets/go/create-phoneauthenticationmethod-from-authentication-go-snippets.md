---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d4291c397bea3c51d87aa947f833221d2feb5e9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327657"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPhoneAuthenticationMethod()
phoneNumber := "+1 2065555555"
requestBody.SetPhoneNumber(&phoneNumber)
phoneType := "mobile"
requestBody.SetPhoneType(&phoneType)
result, err := graphClient.Me().Authentication().PhoneMethods().Post(requestBody)


```