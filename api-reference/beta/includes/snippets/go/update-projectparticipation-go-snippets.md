---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e94e29f6cd87e2982f52e7c9a9f1880f9689260
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094222"
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
graphClient.Me().Profile().ProjectsById(&projectParticipationId).Patch(options)


```