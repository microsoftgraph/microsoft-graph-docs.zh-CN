---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e03468eb2645acaecaa28ed0581987636ab662b3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865737"
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