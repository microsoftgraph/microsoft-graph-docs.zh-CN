---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef0b6d7cdc8cd55ccb0802e96662422800f05800
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093450"
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
graphClient.Print().SharesById(&printerShareId).Patch(options)


```