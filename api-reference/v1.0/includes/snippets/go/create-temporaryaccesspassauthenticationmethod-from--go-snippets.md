---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3613a79ca820cc1317acde244cb55e24b17456a9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093335"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTemporaryAccessPassAuthenticationMethod()
startDateTime, err := time.Parse(time.RFC3339, "2022-06-05T00:00:00.000Z")
requestBody.SetStartDateTime(&startDateTime)
lifetimeInMinutes := int32(60)
requestBody.SetLifetimeInMinutes(&lifetimeInMinutes)
isUsableOnce := false
requestBody.SetIsUsableOnce(&isUsableOnce)
userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethods().Post(requestBody)


```