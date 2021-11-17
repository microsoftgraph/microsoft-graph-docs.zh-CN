---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaa74fd9e4e082fce26ed6a03a9ac1218ad28846bf70fc997cc939772d6669e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903129"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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