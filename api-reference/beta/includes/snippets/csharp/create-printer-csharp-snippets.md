---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 99736a6c7acb4e5b9feef43b25d4fd9d6970b93e
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/11/2020
ms.locfileid: "48994519"
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