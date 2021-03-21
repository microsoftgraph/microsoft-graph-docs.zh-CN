---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22b4eed9fe0ee7275119c52faf8e59d62060a006
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980041"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("start", "2018-04-30T00:00:00Z"));
requestOptions.add(new QueryOption("end", "2018-05-10T00:00:00Z"));

BookingAppointmentCollectionPage calendarView = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").calendarView()
    .buildRequest( requestOptions )
    .get();

```