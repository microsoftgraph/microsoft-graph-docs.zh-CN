---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0914a8d37d661418d8c1b9d6255a0222fed4f62
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412072"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2cAuthenticationMethodsPolicy()
isEmailPasswordAuthenticationEnabled := false
requestBody.SetIsEmailPasswordAuthenticationEnabled(&isEmailPasswordAuthenticationEnabled)
isUserNameAuthenticationEnabled := true
requestBody.SetIsUserNameAuthenticationEnabled(&isUserNameAuthenticationEnabled)
isPhoneOneTimePasswordAuthenticationEnabled := true
requestBody.SetIsPhoneOneTimePasswordAuthenticationEnabled(&isPhoneOneTimePasswordAuthenticationEnabled)
options := &msgraphsdk.B2cAuthenticationMethodsPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().B2cAuthenticationMethodsPolicy().Patch(options)


```