---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f7185ffad11c7cb47fb88a629e125bff6061235a0300c2a86a2710bae333e1c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902397"
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