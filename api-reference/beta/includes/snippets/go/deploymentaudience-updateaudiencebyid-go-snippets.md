---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 285a0622319544440e9b9522f1e802d08b07fcb3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029944"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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