---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f06c373f51c16cfbae381e64fdf762f416bc582046a6a26d4f631aa59d79d653
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277294"
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