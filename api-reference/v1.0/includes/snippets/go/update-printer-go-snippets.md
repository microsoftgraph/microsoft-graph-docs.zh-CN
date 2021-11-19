---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ff687e089bfb18ae1b11d9decbc4ccc4753c933
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101832"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrinter()
location := msgraphsdk.NewPrinterLocation()
requestBody.SetLocation(location)
latitude := float64(1.1)
location.SetLatitude(&latitude)
longitude := float64(2.2)
location.SetLongitude(&longitude)
altitudeInMeters := int32(3)
location.SetAltitudeInMeters(&altitudeInMeters)
requestBody.SetAdditionalData(map[string]interface{}{
    "name": "PrinterName",
}
options := &msgraphsdk.PrinterRequestBuilderPatchOptions{
    Body: requestBody,
}
printerId := "printer-id"
graphClient.Print().PrintersById(&printerId).Patch(options)


```