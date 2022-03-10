---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a8244035451585da9ac28f26e806107996166c7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411906"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewLanguageProficiency()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
options := &msgraphsdk.LanguageProficiencyRequestBuilderPatchOptions{
    Body: requestBody,
}
languageProficiencyId := "languageProficiency-id"
result, err := graphClient.Me().Profile().LanguagesById(&languageProficiencyId).Patch(options)


```