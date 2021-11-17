---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecdc9b56555cd1ba7a010c00d8fceb0be3c9bc72a157efc3e64d907a91b06ba8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105036"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers["{bookingCustomer-id}"]
    .Request()
    .DeleteAsync();

```