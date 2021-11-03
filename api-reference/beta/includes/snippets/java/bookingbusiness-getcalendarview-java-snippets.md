---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9604ca82a0032c6c455f6eef92e58cc30494362b4d7cd8669d6818ef7ea4e41
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162109"
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