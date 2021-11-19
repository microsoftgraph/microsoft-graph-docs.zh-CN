---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfbd615ca28e09689843b6536819978e22bcc7c8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098767"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewApplication()
displayName := "Display name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ApplicationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Applications().Post(options)


```