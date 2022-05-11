---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ce5967dd22b654e522bfad7147593cd1179ffb7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329240"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
memberId := "319b41e8-d9e4-42f8-bdc9-741113f48b33"
requestBody.SetMemberId(&memberId)
membershipRule := "(user.displayName -startsWith "EndTestUser")"
requestBody.SetMembershipRule(&membershipRule)
result, err := graphClient.Groups().EvaluateDynamicMembership().Post(requestBody)


```