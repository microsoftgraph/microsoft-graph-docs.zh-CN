---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ec8eb16e75ca5807b3e1915211cf2e85e0a7efb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090897"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrinterShare()
displayName := "ShareName"
requestBody.SetDisplayName(&displayName)
allowAllUsers := true
requestBody.SetAllowAllUsers(&allowAllUsers)
requestBody.SetAdditionalData(map[string]interface{}{
    "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}",
}
options := &msgraphsdk.PrinterShareRequestBuilderPatchOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
graphClient.Print().SharesById(&printerShareId).Patch(options)


```