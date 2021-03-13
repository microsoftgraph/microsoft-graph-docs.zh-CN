---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4dcbc7b5de41eb6147d6b8e153e354bf65562888
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776982"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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