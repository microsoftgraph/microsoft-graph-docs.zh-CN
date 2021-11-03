---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e664a71c073a9846ad7fa31d69f62deab7827f8c5c716cd0bdc61844464dc28f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162303"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingService bookingService = new BookingService();
bookingService.defaultDuration = DatatypeFactory.newInstance().newDuration("PT30M");

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").services("57da6774-a087-4d69-b0e6-6fb82c339976")
    .buildRequest()
    .patch(bookingService);

```