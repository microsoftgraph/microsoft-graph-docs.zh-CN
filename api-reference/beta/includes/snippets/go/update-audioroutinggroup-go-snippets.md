---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8e1b4a2d1bca10db7f58468ad8c810a9bd2fd19
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995327"
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
    "72f988bf-86f1-41af-91ab-2d7cd011db47",
}
options := &msgraphsdk.AudioRoutingGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
callId := "call-id"
audioRoutingGroupId := "audioRoutingGroup-id"
graphClient.Communications().CallsById(&callId).AudioRoutingGroupsById(&audioRoutingGroupId).Patch(options)


```