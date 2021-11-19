---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 661e1d18e4f7a5c773aea0bcd2f3e45e2f2a83aa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103546"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetGroupIds( []String {
    "groupIds-value",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().CheckMemberGroups().Post(options)


```