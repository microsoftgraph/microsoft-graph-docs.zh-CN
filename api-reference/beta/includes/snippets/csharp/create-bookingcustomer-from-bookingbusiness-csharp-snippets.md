---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9c5b6974cc438a11ef4ffccde80a9c0c5444c5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = new BookingCustomer
{
    DisplayName = "Joni Sherman",
    EmailAddress = "jonis@relecloud.com"
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers
    .Request()
    .AddAsync(bookingCustomer);

```