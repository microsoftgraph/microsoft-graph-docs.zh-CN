---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e03468eb2645acaecaa28ed0581987636ab662b3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960789"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("start", "2018-04-30T00:00:00Z"));
requestOptions.add(new QueryOption("end", "2018-05-10T00:00:00Z"));

IBookingAppointmentCollectionPage calendarView = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").calendarView()
    .buildRequest( requestOptions )
    .get();

```