---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c1347248fb5972415984556c437562f1b677e03
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960430"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingService bookingService = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").services("57da6774-a087-4d69-b0e6-6fb82c339976")
    .buildRequest()
    .get();

```