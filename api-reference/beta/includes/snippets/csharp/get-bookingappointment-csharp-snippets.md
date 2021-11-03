---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aec501143d22a44c57766ef28df45b4572175379f12a218fece36fed211722fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingAppointment = await graphClient.BookingBusinesses["{bookingBusiness-id}"].Appointments["{bookingAppointment-id}"]
    .Request()
    .GetAsync();

```