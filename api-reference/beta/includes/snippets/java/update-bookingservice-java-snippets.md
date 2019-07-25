---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 646c4ae929db8b4956325a976777ed23010b4535
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865264"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingService bookingService = new BookingService();
bookingService.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.bookingService"));
bookingService.defaultDuration = "PT30M";

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").services("57da6774-a087-4d69-b0e6-6fb82c339976")
    .buildRequest()
    .patch(bookingService);

```