---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97128d952897db59d523762aed74aea98631a181
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983017"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKoAAA=")
    .cancel(BookingAppointmentCancelParameterSet
        .newBuilder()
        .withCancellationMessage(cancellationMessage)
        .build())
    .buildRequest()
    .post();

```