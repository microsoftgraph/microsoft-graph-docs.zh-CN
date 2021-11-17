---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c9c197928536b4a246290c0fbc39839a0f0df2a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.OnPremisesAgentRequestBuilderGetQueryParameters{
    Expand: "agentGroups",
}
options := &msgraphsdk.OnPremisesAgentRequestBuilderGetOptions{
    Q: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
onPremisesAgentId := "onPremisesAgent-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentsById(&onPremisesAgentId).Get(options)


```