---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 743d43df82a64ed9607310dfa85a4a1437bb0c0c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865444"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = new BookingBusiness();
bookingBusiness.email = "admin@fabrikam.com";
BookingSchedulingPolicy schedulingPolicy = new BookingSchedulingPolicy();
schedulingPolicy.timeSlotInterval = "PT60M";
schedulingPolicy.minimumLeadTime = "P1D";
schedulingPolicy.maximumAdvance = "P30D";
schedulingPolicy.sendConfirmationsToOwner = true;
schedulingPolicy.allowStaffSelection = true;
bookingBusiness.schedulingPolicy = schedulingPolicy;

graphClient.bookingBusinesses("fabrikam@M365B489948.onmicrosoft.com")
    .buildRequest()
    .patch(bookingBusiness);

```