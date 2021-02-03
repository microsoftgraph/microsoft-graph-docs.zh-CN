---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14e9c53d43f6ebd1a9b40ccf60fbcbbcfdaabd63
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093666"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnector printConnector = new PrintConnector();
printConnector.name = "ConnectorName";
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