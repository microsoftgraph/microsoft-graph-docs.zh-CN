---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ce364a0aa5fd0cf5fb99c844b22b8b8b8ce51b608760379552a46816373775e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162017"
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

graphClient.print().connectors("{printConnectorId}")
    .buildRequest()
    .patch(printConnector);

```