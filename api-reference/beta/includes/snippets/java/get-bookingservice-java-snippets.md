---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f33de1967822600aadb926915ff42455bcaeec7e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109625"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingService bookingService = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").services("57da6774-a087-4d69-b0e6-6fb82c339976")
    .buildRequest()
    .get();

```