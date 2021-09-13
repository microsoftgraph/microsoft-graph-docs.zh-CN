---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c858b991e1267896ae9259ce8715b39f070da9440c056295be644b96050b0d9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163508"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "I won't be able to make this week. How about next week?";

Boolean sendResponse = true;

TimeSlot proposedNewTime = new TimeSlot();
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2019-12-02T18:00:00";
start.timeZone = "Pacific Standard Time";
proposedNewTime.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2019-12-02T19:00:00";
end.timeZone = "Pacific Standard Time";
proposedNewTime.end = end;

graphClient.me().events("{id}")
    .decline(EventDeclineParameterSet
        .newBuilder()
        .withComment(comment)
        .withSendResponse(sendResponse)
        .withProposedNewTime(proposedNewTime)
        .build())
    .buildRequest()
    .post();

```