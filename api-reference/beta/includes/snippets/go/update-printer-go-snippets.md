---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f8e5de3af43951631d67b42d0e200248ecf4f0d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412290"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrinter()
name := "PrinterName"
requestBody.SetName(&name)
location := msgraphsdk.NewPrinterLocation()
requestBody.SetLocation(location)
latitude := float64(1.1)
location.SetLatitude(&latitude)
longitude := float64(2.2)
location.SetLongitude(&longitude)
altitudeInMeters := int32(3)
location.SetAltitudeInMeters(&altitudeInMeters)
options := &msgraphsdk.PrinterRequestBuilderPatchOptions{
    Body: requestBody,
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Patch(options)


```