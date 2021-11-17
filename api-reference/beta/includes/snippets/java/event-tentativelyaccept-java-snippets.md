---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a438ddabb63aafdcace6f1916de8b7ebff745ae623c5dd176e619bd5327692e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277335"
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