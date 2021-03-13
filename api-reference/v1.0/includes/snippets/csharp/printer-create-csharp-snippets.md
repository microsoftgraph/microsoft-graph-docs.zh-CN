---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99736a6c7acb4e5b9feef43b25d4fd9d6970b93e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Test Printer";

var manufacturer = "Test Printer Manufacturer";

var model = "Test Printer Model";

String physicalDeviceId = null;

var hasPhysicalDevice = false;

var certificateSigningRequest = new PrintCertificateSigningRequestObject
{
    Content = "{content}",
    TransportKey = "{sampleTransportKey}"
};

String connectorId = null;

await graphClient.Print.Printers
    .Create(displayName,manufacturer,model,certificateSigningRequest,physicalDeviceId,hasPhysicalDevice,connectorId)
    .Request()
    .PostAsync();

```