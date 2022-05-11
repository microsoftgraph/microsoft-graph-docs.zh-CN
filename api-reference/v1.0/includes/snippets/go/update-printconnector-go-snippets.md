---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a1e4693d18e89149547ec1e676ad86b1e956d52
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326614"
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
printConnectorId := "printConnector-id"
graphClient.Print().ConnectorsById(&printConnectorId).Patch(requestBody)


```