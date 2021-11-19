---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c303ad4380a9f17dc57338e2d3ca3c088feb7c1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091484"
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
graphClient.Policies().B2cAuthenticationMethodsPolicy().Patch(options)


```