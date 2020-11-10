---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4334e1e6510c8b7f0813de803661324c8c341076
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960687"
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