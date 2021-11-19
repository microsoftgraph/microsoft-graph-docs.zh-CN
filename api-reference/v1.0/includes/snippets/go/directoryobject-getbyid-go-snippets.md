---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cca4f445de17858ca9f278c4bb0f4772a23f10d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100158"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetIds( []String {
    "84b80893874940a3-97b7-68513b600544",
    "5d6059b6368d-45f8-91e18e07d485f1d0",
}
requestBody.SetTypes( []String {
    "user",
}
options := &msgraphsdk.GetByIdsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DirectoryObjects().GetByIds().Post(options)


```