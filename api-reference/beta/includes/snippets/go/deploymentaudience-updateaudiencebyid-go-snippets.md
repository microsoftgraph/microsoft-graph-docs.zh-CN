---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 424f521e781fb51b9001dfeee2aeb2c40d50ff14
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084359"
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
options := &msgraphsdk.UpdateAudienceByIdRequestBuilderPostOptions{
    Body: requestBody,
}
deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Audience().UpdateAudienceById().Post(options)


```