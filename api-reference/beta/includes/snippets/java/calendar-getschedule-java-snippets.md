---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec7c00675cd4572e61b31f07278bd354890b18a0
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396721"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .getSchedule(schedulesList,endTime,startTime,availabilityViewInterval)
    .buildRequest( requestOptions )
    .post();

```