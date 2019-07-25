---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 45e75108b950ad2fb5c6763fe17fef8e84e2fe8f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709551"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = new BookingCustomer
{
    DisplayName = "Joni Sherman",
    EmailAddress = "jonis@relecloud.com"
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Customers
    .Request()
    .AddAsync(bookingCustomer);

```