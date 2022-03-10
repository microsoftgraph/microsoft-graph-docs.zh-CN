---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c20468ac66c28db376bcaf92a646486852df2c0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412413"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOnPremisesAgentGroup()
displayName := "Group New Name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.OnPremisesAgentGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
onPremisesAgentGroupId := "onPremisesAgentGroup-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentGroupsById(&onPremisesAgentGroupId).Patch(options)


```