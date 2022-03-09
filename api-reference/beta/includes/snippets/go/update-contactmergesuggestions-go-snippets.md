---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56bff72bdde8eb18eb245cdd399412fbd73bee6b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395095"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactMergeSuggestions()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.ContactMergeSuggestionsRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Settings().ContactMergeSuggestions().Patch(options)


```