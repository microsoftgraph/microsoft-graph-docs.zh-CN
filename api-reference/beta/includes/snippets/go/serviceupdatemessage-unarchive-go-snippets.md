---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40c998bcf84ef2c762661f6df444312b0d375daa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099760"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetMessageIds( []String {
    "MC172851",
    "MC167983",
}
options := &msgraphsdk.UnarchiveRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Admin().ServiceAnnouncement().Messages().Unarchive().Post(options)


```