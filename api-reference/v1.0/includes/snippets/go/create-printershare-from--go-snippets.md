---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e109bc0d8e7c0137255c49df074510a225cc19a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095248"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrinterShare()
displayName := "ShareName"
requestBody.SetDisplayName(&displayName)
allowAllUsers := false
requestBody.SetAllowAllUsers(&allowAllUsers)
requestBody.SetAdditionalData(map[string]interface{}{
    "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}",
}
options := &msgraphsdk.SharesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Print().Shares().Post(options)


```