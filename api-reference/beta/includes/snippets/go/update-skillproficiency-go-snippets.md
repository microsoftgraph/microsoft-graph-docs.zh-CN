---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c15e1bd70331deb9172678c75882fae8157f9f7e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412710"
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
result, err := graphClient.Me().Profile().SkillsById(&skillProficiencyId).Patch(options)


```