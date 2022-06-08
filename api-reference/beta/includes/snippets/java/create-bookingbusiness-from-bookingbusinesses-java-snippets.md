---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0defe980e4f32d681a82f8a4e4a738be0273cb6
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946831"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = new BookingBusiness();
bookingBusiness.displayName = "Fourth Coffee";
PhysicalAddress address = new PhysicalAddress();
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