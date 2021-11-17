---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e6afa7ddf21627bdfc3e966e3e8fdce1e554943
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985289"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
graphClient.Print().ConnectorsById(&printConnectorId).Patch(options)


```