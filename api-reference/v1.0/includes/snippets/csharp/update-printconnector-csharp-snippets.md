---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f34927f7045ffa6bff049b7724a11ce31375f82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = new PrintConnector
{
    DisplayName = "ConnectorName",
    FullyQualifiedDomainName = "CONNECTOR-MACHINE",
    OperatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
    AppVersion = "0.19.7338.23496",
    Location = new PrinterLocation
    {
        Latitude = 1.1,
        Longitude = 2.2,
        AltitudeInMeters = 3
    }
};

await graphClient.Print.Connectors["{printConnector-id}"]
    .Request()
    .UpdateAsync(printConnector);

```