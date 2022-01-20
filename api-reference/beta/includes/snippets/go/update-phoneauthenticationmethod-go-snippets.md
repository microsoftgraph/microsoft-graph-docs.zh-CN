---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 332266bee4db5f819188793f2a65b7c50c1d5955
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137708"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "phoneNumber": "+1 2065555554",
    "phoneType": "mobile",
}
options := &msgraphsdk.PhoneAuthenticationMethodRequestBuilderPutOptions{
    Body: requestBody,
}
phoneAuthenticationMethodId := "phoneAuthenticationMethod-id"
graphClient.Me().Authentication().PhoneMethodsById(&phoneAuthenticationMethodId).Put(options)


```