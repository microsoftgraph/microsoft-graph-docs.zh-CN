---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50ed348b8c08266195d51ea8503238650ceadf82
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960550"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = new BookingBusiness();
bookingBusiness.email = "admin@fabrikam.com";
BookingSchedulingPolicy schedulingPolicy = new BookingSchedulingPolicy();
schedulingPolicy.timeSlotInterval = DatatypeFactory.newInstance().newDuration("PT60M");
schedulingPolicy.minimumLeadTime = DatatypeFactory.newInstance().newDuration("P1D");
schedulingPolicy.maximumAdvance = DatatypeFactory.newInstance().newDuration("P30D");
schedulingPolicy.sendConfirmationsToOwner = true;
schedulingPolicy.allowStaffSelection = true;
bookingBusiness.schedulingPolicy = schedulingPolicy;

graphClient.bookingBusinesses("fabrikam@M365B489948.onmicrosoft.com")
    .buildRequest()
    .patch(bookingBusiness);

```