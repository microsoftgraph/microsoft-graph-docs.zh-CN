---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 275df1e428cabb978c19685fd644cb63e33b34a7
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093645"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = new Printer();
printer.name = "PrinterName";
PrinterLocation location = new PrinterLocation();
location.latitude = 1.1d;
location.longitude = 2.2d;
location.altitudeInMeters = 3;
printer.location = location;

graphClient.print().printers("{id}")
    .buildRequest()
    .patch(printer);

```