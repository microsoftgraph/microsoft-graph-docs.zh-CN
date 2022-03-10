---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d15db32ee5ed024f52700f785e1e86403e16f058
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412351"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProjectParticipation()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
client := msgraphsdk.NewCompanyDetail()
requestBody.SetClient(client)
department := "Corporate Marketing"
client.SetDepartment(&department)
webUrl := "https://www.contoso.com"
client.SetWebUrl(&webUrl)
options := &msgraphsdk.ProjectParticipationRequestBuilderPatchOptions{
    Body: requestBody,
}
projectParticipationId := "projectParticipation-id"
result, err := graphClient.Me().Profile().ProjectsById(&projectParticipationId).Patch(options)


```