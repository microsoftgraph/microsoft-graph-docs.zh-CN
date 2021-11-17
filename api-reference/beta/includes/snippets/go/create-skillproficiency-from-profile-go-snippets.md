---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c650f8a3124dd9723e0ddabfd9d298a765b97848
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980067"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.SkillsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Skills().Post(options)


```