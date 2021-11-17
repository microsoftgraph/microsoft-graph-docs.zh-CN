---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f089e626ee9e3d318e5a9079b423afaef6c71bb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009944"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetGroupIds( []String {
    "groupIds-value",
}
options := &msgraphsdk.CheckMemberGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().CheckMemberGroups().Post(options)


```