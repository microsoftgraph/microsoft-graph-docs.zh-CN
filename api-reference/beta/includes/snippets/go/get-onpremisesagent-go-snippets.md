---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cae2c502d634f8d3586f04cc8e07ca1f25259bcc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090252"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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