---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aef41d74e1f63d33b2efe1ddabd6036c39f9ae7b4af0c4475a72cb29670e9837
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903118"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = new BookingCustomer
{
    DisplayName = "Adele",
    EmailAddress = "adele@relecloud.com"
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers["{bookingCustomer-id}"]
    .Request()
    .UpdateAsync(bookingCustomer);

```