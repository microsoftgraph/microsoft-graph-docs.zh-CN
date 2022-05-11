---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c1395aba41f106a1c54b39041c4220156d00a19
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328566"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
memberEntityType := "String"
requestBody.SetMemberEntityType(&memberEntityType)
requestBody.SetAddMembers( []String {
    "String",
}
requestBody.SetRemoveMembers( []String {
    "String",
}
requestBody.SetAddExclusions( []String {
    "String",
}
requestBody.SetRemoveExclusions( []String {
    "String",
}
deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Audience().UpdateAudienceById(deployment-id).Post(requestBody)


```