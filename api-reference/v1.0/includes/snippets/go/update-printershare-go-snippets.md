---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6738b3d23b7733918c1c3389e75577a0e3553e1e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412642"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrinterShare()
displayName := "PrinterShare Name"
requestBody.SetDisplayName(&displayName)
allowAllUsers := false
requestBody.SetAllowAllUsers(&allowAllUsers)
requestBody.SetAdditionalData(map[string]interface{}{
    "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}",
}
options := &msgraphsdk.PrinterShareRequestBuilderPatchOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).Patch(options)


```