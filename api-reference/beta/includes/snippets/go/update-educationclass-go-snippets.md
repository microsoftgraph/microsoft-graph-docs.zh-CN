---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91e5157845d0a64c41dc7861e305add7b6336237
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412683"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationClass()
description := "History - World History 1"
requestBody.SetDescription(&description)
displayName := "World History Level 1"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.EducationClassRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Patch(options)


```