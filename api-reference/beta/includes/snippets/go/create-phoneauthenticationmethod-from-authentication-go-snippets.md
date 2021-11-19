---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fd1dd2c7aeea7a09bcd9447f9691b4c9440a131
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090672"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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