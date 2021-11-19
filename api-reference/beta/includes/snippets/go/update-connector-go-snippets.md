---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3690952566e738ce43df0e4827c0eb0a04263d1b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088364"
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
graphClient.Print().ConnectorsById(&printConnectorId).Patch(options)


```