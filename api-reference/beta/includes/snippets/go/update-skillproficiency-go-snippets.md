---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06e6444844085f6fee291d71a5c6917b1fe443cd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101472"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSkillProficiency()
requestBody.SetCategories( []String {
    "Professional",
}
proficiency := "advancedProfessional"
requestBody.SetProficiency(&proficiency)
options := &msgraphsdk.SkillProficiencyRequestBuilderPatchOptions{
    Body: requestBody,
}
skillProficiencyId := "skillProficiency-id"
graphClient.Me().Profile().SkillsById(&skillProficiencyId).Patch(options)


```