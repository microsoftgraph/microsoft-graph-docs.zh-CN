---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f9bffef91b731d457f5c1b6679819dbc72696f7d37d93a7eb3de4851235ed77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103907"
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