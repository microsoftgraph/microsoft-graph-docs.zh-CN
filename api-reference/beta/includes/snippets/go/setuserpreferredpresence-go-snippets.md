---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7b56ac1975e66eaaf19ef7a936105d4d3da8278
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328732"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
availability := "DoNotDisturb"
requestBody.SetAvailability(&availability)
activity := "DoNotDisturb"
requestBody.SetActivity(&activity)
expirationDuration := "PT8H"
requestBody.SetExpirationDuration(&expirationDuration)
userId := "user-id"
graphClient.UsersById(&userId).Presence().SetUserPreferredPresence(user-id).Post(requestBody)


```