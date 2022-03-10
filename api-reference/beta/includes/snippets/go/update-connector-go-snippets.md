---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a480727c153b222f850f77e186a93952a0e5935
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412714"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrintConnector()
displayName := "ConnectorName"
requestBody.SetDisplayName(&displayName)
fullyQualifiedDomainName := "CONNECTOR-MACHINE"
requestBody.SetFullyQualifiedDomainName(&fullyQualifiedDomainName)
operatingSystem := "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555"
requestBody.SetOperatingSystem(&operatingSystem)
appVersion := "0.19.7338.23496"
requestBody.SetAppVersion(&appVersion)
location := msgraphsdk.NewPrinterLocation()
requestBody.SetLocation(location)
latitude := float64(1.1)
location.SetLatitude(&latitude)
longitude := float64(2.2)
location.SetLongitude(&longitude)
altitudeInMeters := int32(3)
location.SetAltitudeInMeters(&altitudeInMeters)
options := &msgraphsdk.PrintConnectorRequestBuilderPatchOptions{
    Body: requestBody,
}
printConnectorId := "printConnector-id"
result, err := graphClient.Print().ConnectorsById(&printConnectorId).Patch(options)


```