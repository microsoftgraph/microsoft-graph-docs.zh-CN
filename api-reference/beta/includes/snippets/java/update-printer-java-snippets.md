---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f54b9a6078b7323fe88d9d076e6910bf4ef6a312b9494e8d3160637825a1f53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902386"
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