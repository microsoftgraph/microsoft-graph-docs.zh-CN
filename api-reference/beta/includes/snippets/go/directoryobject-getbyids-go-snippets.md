---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f2ef447f399e379e4d52b99f70727b7302921fe
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097400"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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