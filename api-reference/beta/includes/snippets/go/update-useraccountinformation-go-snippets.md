---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 337fa095dc8c4bcb5439e1836ac98f04dc63d380
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411640"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserAccountInformation()
countryCode := "NO"
requestBody.SetCountryCode(&countryCode)
options := &msgraphsdk.UserAccountInformationRequestBuilderPatchOptions{
    Body: requestBody,
}
userAccountInformationId := "userAccountInformation-id"
result, err := graphClient.Me().Profile().AccountById(&userAccountInformationId).Patch(options)


```