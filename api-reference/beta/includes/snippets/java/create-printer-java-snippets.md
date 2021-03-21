---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ab7704f32c695d3ec2f2fc6fd7719a2ee16654a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978032"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Test Printer";

String manufacturer = "Test Printer Manufacturer";

String model = "Test Printer Model";



Boolean hasPhysicalDevice = false;

PrintCertificateSigningRequest certificateSigningRequest = new PrintCertificateSigningRequest();
certificateSigningRequest.content = "{content}";
certificateSigningRequest.transportKey = "{sampleTransportKey}";



graphClient.print().printers()
    .create(PrinterCreateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withManufacturer(manufacturer)
        .withModel(model)
        .withPhysicalDeviceId(physicalDeviceId)
        .withHasPhysicalDevice(hasPhysicalDevice)
        .withCertificateSigningRequest(certificateSigningRequest)
        .withConnectorId(connectorId)
        .build())
    .buildRequest()
    .post();

```