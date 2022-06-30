---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3613a79ca820cc1317acde244cb55e24b17456a9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438058"
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