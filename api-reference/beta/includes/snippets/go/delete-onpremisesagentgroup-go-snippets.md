---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 169e201c04291d342a71451cb2c245592e4c7e13
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411813"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
onPremisesAgentGroupId := "onPremisesAgentGroup-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentGroupsById(&onPremisesAgentGroupId).Delete(nil)


```