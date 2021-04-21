---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66f5eaf8e7d58cca522df824d90a3acfeacba9ed
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921984"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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