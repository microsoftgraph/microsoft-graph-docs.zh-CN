---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c36e46c0113c2190397a4331cacb14e8b6d931b5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102067"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAddLicenses( []AssignedLicense {
}
requestBody.SetRemoveLicenses( []String {
    "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "b05e124f-c7cc-45a0-a6aa-8cf78c946968",
}
options := &msgraphsdk.AssignLicenseRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AssignLicense().Post(options)


```