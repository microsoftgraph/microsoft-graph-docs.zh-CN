---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1b5e7c1327bc8177a36a8eba9a6d4a2ae01619a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = new PrintConnector
{
    Name = "ConnectorName",
    FullyQualifiedDomainName = "CONNECTOR-MACHINE",
    OperatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
    AppVersion = "0.19.7338.23496",
    Location = new PrinterLocation
    {
        Latitude = 1.1f,
        Longitude = 2.2f,
        AltitudeInMeters = 3
    }
};

await graphClient.Print.Connectors["{id}"]
    .Request()
    .UpdateAsync(printConnector);

```