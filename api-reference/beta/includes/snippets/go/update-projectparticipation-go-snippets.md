---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ce54ce0bfa08d6a1bd82c2fb325e5f389ba403f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027851"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.Me().Profile().ProjectsById(&projectParticipationId).Patch(options)


```