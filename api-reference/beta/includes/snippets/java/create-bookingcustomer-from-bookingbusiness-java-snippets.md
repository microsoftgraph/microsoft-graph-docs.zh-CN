---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25a9e18cdd4c67213398bdbb01769ce6cd462f8f298f6a5e00d9dbc8dd4c02bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903143"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomer bookingCustomer = new BookingCustomer();
bookingCustomer.displayName = "Joni Sherman";
bookingCustomer.emailAddress = "jonis@relecloud.com";

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers()
    .buildRequest()
    .post(bookingCustomer);

```