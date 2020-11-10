---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25fe3fe72db7acd6d842932d1574daab3f67ea40
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979773"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = new Printer();
printer.name = "PrinterName";
PrinterLocation location = new PrinterLocation();
location.latitude = 1.1;
location.longitude = 2.2;
location.altitudeInMeters = 3;
printer.location = location;

graphClient.print().printers("{id}")
    .buildRequest()
    .patch(printer);

```