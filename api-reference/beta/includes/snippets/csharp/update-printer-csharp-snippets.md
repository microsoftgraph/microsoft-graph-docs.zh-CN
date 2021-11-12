---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf44c44b96e6e4112fbeb21da3f78d7ff368195b29a93171a852d1b699f7df1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101362"
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