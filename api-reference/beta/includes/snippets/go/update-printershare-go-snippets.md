---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 842c6bb6173574024a6f8c4451bc3c0cd77fe6ae
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412752"
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
result, err := graphClient.Print().SharesById(&printerShareId).Patch(options)


```