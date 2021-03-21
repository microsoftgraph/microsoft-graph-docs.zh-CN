---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3e7d93a9f51c1c3e573e5dadc057605720df00a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984356"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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