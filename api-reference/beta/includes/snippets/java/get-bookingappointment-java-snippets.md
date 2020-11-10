---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24841a87af3cf561ca77ce9cf35f0cd722830d51
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960934"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointment bookingAppointment = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKnAAA=")
    .buildRequest()
    .get();

```