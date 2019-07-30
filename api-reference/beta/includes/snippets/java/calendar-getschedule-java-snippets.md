---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ca13dc4520016c3f18641abab1366925e8c57c0
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35930910"
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

String availabilityViewInterval = "60";

graphClient.me().calendar()
    .getschedule(schedulesList,endTime,startTime,availabilityViewInterval)
    .buildRequest( requestOptions )
    .post();

```