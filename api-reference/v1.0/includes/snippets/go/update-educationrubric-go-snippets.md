---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7db7998e91758228404dfcf1128d96e89f3964a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006214"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationRubric()
displayName := "Example Credit Rubric after display name patch"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.EducationRubricRequestBuilderPatchOptions{
    Body: requestBody,
}
educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Patch(options)


```