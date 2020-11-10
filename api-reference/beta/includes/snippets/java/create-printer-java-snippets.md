---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 294bd4cda4104322fedba31ea1f5e6f9b9f7c16d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972466"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Test Printer";

String manufacturer = "Test Printer Manufacturer";

String model = "Test Printer Model";



Boolean hasPhysicalDevice = false;

PrintCertificateSigningRequest certificateSigningRequest = new PrintCertificateSigningRequest();
certificateSigningRequest.content = "{content}";
certificateSigningRequest.transportKey = "{sampleTransportKey}";



graphClient.print().printers()
    .create(displayName,manufacturer,model,physicalDeviceId,hasPhysicalDevice,certificateSigningRequest,connectorId)
    .buildRequest()
    .post();

```