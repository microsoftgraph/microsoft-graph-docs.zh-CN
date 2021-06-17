---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0c7385700787726faf8ae11e1ab9c3319ab83f7
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992239"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "I may not be able to make this week. How about next week?";

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
    .tentativelyAccept(EventTentativelyAcceptParameterSet
        .newBuilder()
        .withComment(comment)
        .withSendResponse(sendResponse)
        .withProposedNewTime(proposedNewTime)
        .build())
    .buildRequest()
    .post();

```