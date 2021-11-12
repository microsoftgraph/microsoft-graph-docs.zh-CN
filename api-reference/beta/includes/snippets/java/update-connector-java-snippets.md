---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61e9d53ec754f4b305ebd464715f6f192365f702eb4774474d8259d38f490304
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277293"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnector printConnector = new PrintConnector();
printConnector.displayName = "ConnectorName";
printConnector.fullyQualifiedDomainName = "CONNECTOR-MACHINE";
printConnector.operatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555";
printConnector.appVersion = "0.19.7338.23496";
PrinterLocation location = new PrinterLocation();
location.latitude = 1.1d;
location.longitude = 2.2d;
location.altitudeInMeters = 3;
printConnector.location = location;

graphClient.print().connectors("{id}")
    .buildRequest()
    .patch(printConnector);

```