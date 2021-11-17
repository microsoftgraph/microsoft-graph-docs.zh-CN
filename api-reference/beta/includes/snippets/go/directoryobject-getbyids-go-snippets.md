---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3d520d529a9aaaf70ac8ca5546c4af9714a6c9d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005359"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetIds( []String {
    "84b80893-8749-40a3-97b7-68513b600544",
    "5d6059b6-368d-45f8-91e1-8e07d485f1d0",
}
requestBody.SetTypes( []String {
    "user",
}
options := &msgraphsdk.GetByIdsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DirectoryObjects().GetByIds().Post(options)


```