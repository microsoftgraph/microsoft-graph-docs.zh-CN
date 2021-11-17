---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b34c390bb2124eb592e68d1bfaf0be05f61e1a6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982363"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPhoneAuthenticationMethod()
phoneNumber := "+1 2065555555"
requestBody.SetPhoneNumber(&phoneNumber)
phoneType := "mobile"
requestBody.SetPhoneType(&phoneType)
options := &msgraphsdk.PhoneMethodsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Authentication().PhoneMethods().Post(options)


```