---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9520921e4293107dd5fffcef803d0e05f9ec0a2c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAudioRoutingGroup()
id := "oneToOne"
requestBody.SetId(&id)
routingMode := "oneToOne"
requestBody.SetRoutingMode(&routingMode)
requestBody.SetSources( []String {
    "632899f8-2ea1-4604-8413-27bd2892079f",
}
requestBody.SetReceivers( []String {
    "550fae72-d251-43ec-868c-373732c2704f",
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).AudioRoutingGroups().Post(requestBody)


```