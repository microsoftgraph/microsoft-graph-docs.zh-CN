---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bced586eae643a99b546e27cae6372d09f432e08327d5de1326ef2c712e9a0c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331847"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

LinkedList<String> schedulesList = new LinkedList<String>();
schedulesList.add("adelev@contoso.onmicrosoft.com");
schedulesList.add("meganb@contoso.onmicrosoft.com");

DateTimeTimeZone startTime = new DateTimeTimeZone();
startTime.dateTime = "2019-03-15T09:00:00";
startTime.timeZone = "Pacific Standard Time";

DateTimeTimeZone endTime = new DateTimeTimeZone();
endTime.dateTime = "2019-03-15T18:00:00";
endTime.timeZone = "Pacific Standard Time";

int availabilityViewInterval = 60;

graphClient.me().calendar()
    .getSchedule(CalendarGetScheduleParameterSet
        .newBuilder()
        .withSchedules(schedulesList)
        .withEndTime(endTime)
        .withStartTime(startTime)
        .withAvailabilityViewInterval(availabilityViewInterval)
        .build())
    .buildRequest( requestOptions )
    .post();

```