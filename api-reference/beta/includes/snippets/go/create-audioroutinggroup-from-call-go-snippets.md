---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7454dacac445b536be4fac82659b7b5fb9e4caea
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018870"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.AudioRoutingGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).AudioRoutingGroups().Post(options)


```