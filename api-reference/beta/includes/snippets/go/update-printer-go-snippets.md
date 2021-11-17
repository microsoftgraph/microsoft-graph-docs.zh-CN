---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dcd7dd4af617c1bbf7e53e728a40b3992648127
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980409"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.Print().PrintersById(&printerId).Patch(options)


```