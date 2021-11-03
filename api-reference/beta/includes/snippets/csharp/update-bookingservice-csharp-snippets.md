---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 160f99cd0b2ecf3926af01fd28aa46c1900c4ea9dfe1067be268d851b09f62fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162302"
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