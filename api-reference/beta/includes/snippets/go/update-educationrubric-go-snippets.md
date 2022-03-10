---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cb8d274afcf127f9817cc9d4bf89b5f11f6bf14
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412045"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationRubric()
displayName := "Example Credit Rubric after display name patch"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.EducationRubricRequestBuilderPatchOptions{
    Body: requestBody,
}
educationRubricId := "educationRubric-id"
result, err := graphClient.Education().Me().RubricsById(&educationRubricId).Patch(options)


```