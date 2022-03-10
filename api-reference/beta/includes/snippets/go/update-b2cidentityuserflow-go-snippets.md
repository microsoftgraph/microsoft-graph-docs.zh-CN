---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adfb277f22ae8467a55598aacdc2e1c0259397c2
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411821"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewB2cIdentityUserFlow()
isLanguageCustomizationEnabled := true
requestBody.SetIsLanguageCustomizationEnabled(&isLanguageCustomizationEnabled)
defaultLanguageTag := "en"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
options := &msgraphsdk.B2cIdentityUserFlowRequestBuilderPatchOptions{
    Body: requestBody,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).Patch(options)


```