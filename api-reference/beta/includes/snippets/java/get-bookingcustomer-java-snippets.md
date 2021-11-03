---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47447fb2f2c7f3a40a8ada3acffa00cfe0c69475037cbabcbe2ad2be57d6cbb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903837"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomer bookingCustomer = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers("8bb19078-0f45-4efb-b2c5-da78b860f73a")
    .buildRequest()
    .get();

```