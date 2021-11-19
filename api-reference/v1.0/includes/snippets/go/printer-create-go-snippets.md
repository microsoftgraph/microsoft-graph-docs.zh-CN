---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11346e0879fe4664dc16260fbc4d2c629b9235c4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103453"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
displayName := "Test Printer"
requestBody.SetDisplayName(&displayName)
manufacturer := "Test Printer Manufacturer"
requestBody.SetManufacturer(&manufacturer)
model := "Test Printer Model"
requestBody.SetModel(&model)
requestBody.SetPhysicalDeviceId(nil)
hasPhysicalDevice := false
requestBody.SetHasPhysicalDevice(&hasPhysicalDevice)
certificateSigningRequest := msgraphsdk.NewPrintCertificateSigningRequest()
requestBody.SetCertificateSigningRequest(certificateSigningRequest)
content := "{content}"
certificateSigningRequest.SetContent(&content)
transportKey := "{sampleTransportKey}"
certificateSigningRequest.SetTransportKey(&transportKey)
requestBody.SetConnectorId(nil)
options := &msgraphsdk.CreateRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Print().Printers().Create().Post(options)


```