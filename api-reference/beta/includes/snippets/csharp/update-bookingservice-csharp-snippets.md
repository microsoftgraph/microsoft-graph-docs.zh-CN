---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d8580c23c1caa60ed4b04e9782f64d19ac8c294
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingService = new BookingService
{
    DefaultDuration = new Duration("PT30M")
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Services["{bookingService-id}"]
    .Request()
    .UpdateAsync(bookingService);

```