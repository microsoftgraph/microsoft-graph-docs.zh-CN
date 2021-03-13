---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 628cb7b3b24f23dd4745d8ab9efe0608041af413
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = new Printer
{
    Name = "PrinterName",
    Location = new PrinterLocation
    {
        Latitude = 1.1,
        Longitude = 2.2,
        AltitudeInMeters = 3
    }
};

await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .UpdateAsync(printer);

```