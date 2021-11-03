---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f815ef46c75e53bbb5e29bb4ba00f44c77e71da62d10d217bcee1807127a339
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903836"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers["{bookingCustomer-id}"]
    .Request()
    .GetAsync();

```