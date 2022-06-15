---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7b10a3e5eb98a04cbe497a55b3418d93b6f3997
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098719"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalItem()
requestBody.SetAcl( []Acl {
    msgraphsdk.NewAcl(),
type := "everyone"
    SetType(&type)
value := "67a141d8-cf4e-4528-ba07-bed21bfacd2d"
    SetValue(&value)
accessType := "grant"
    SetAccessType(&accessType)
}
externalConnectionId := "externalConnection-id"
externalItemId := "externalItem-id"
graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Patch(requestBody)


```