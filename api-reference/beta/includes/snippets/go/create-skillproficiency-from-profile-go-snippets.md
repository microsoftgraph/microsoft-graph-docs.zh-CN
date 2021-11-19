---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89bd30fbb6d9e8530c854fb2610d5b80f68f12af
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087308"
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
options := &msgraphsdk.SkillsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Skills().Post(options)


```