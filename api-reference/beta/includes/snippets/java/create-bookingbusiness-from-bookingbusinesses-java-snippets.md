---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4334e1e6510c8b7f0813de803661324c8c341076
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865584"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = new BookingBusiness();
bookingBusiness.displayName = "Fourth Coffee";
PhysicalAddress address = new PhysicalAddress();
address.type = PhysicalAddressType.UNKNOWN;
address.postOfficeBox = "P.O. Box 123";
address.street = "4567 Main Street";
address.city = "Buffalo";
address.state = "NY";
address.countryOrRegion = "USA";
address.postalCode = "98052";
bookingBusiness.address = address;
bookingBusiness.phone = "206-555-0100";
bookingBusiness.email = "manager@fourthcoffee.com";
bookingBusiness.webSiteUrl = "https://www.fourthcoffee.com";
bookingBusiness.defaultCurrencyIso = "USD";

graphClient.bookingBusinesses()
    .buildRequest()
    .post(bookingBusiness);

```