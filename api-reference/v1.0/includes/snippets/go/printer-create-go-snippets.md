---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1da7c796a2b66e87400504829c618d0623d5aad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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