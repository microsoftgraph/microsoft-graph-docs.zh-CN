---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45a4f37fd31fab275ab3a0814203eaff38f9138c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326879"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSkillProficiency()
requestBody.SetCategories( []String {
    "Professional",
}
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
displayName := "API Design"
requestBody.SetDisplayName(&displayName)
proficiency := "generalProfessional"
requestBody.SetProficiency(&proficiency)
requestBody.SetCollaborationTags( []String {
    "ableToMentor",
}
result, err := graphClient.Me().Profile().Skills().Post(requestBody)


```