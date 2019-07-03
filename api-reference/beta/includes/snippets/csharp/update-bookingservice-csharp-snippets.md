---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bc954c01a5eb6d9e9f9e9b7656f52b251513d977
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500758"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingService = new BookingService
{
    DefaultDuration = "PT30M"
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Services["57da6774-a087-4d69-b0e6-6fb82c339976"]
    .Request()
    .UpdateAsync(bookingService);

```