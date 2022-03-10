---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bf64ed41164a74fe582b9a5ca5c6c4cf29b69d1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412494"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserIdsRequestBody()
requestBody.SetUserIds( []String {
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345",
}
options := &msgraphsdk.DismissRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.RiskyUsers().Dismiss().Post(options)


```