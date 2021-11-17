---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 925a0eb3e44d22aa14189af882dd945f85a67d2b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002727"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetUserIds( []String {
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345",
}
options := &msgraphsdk.DismissRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.RiskyUsers().Dismiss().Post(options)


```