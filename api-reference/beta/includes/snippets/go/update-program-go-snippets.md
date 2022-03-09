---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad4121c29539217f6a57d5e5119a767c8ad5be3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63398035"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProgram()
displayName := "testprogram3 new name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ProgramRequestBuilderPatchOptions{
    Body: requestBody,
}
programId := "program-id"
result, err := graphClient.ProgramsById(&programId).Patch(options)


```