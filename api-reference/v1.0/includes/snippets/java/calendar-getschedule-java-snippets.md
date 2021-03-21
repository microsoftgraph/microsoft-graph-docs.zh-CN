---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3cc081689e105643d930412f8df0c366ebc5d29
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981599"
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