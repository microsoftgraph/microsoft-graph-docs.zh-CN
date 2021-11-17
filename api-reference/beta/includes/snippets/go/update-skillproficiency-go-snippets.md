---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30c3859ed375e2ec358cb4073c91aa2619fbd6e3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031793"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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