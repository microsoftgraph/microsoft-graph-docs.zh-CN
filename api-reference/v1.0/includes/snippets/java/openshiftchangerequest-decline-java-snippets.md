---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af1792d1981ff558e5bd9f763e734213aececf04
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979108"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "message-value";

graphClient.teams("{id}").schedule().openShiftChangeRequests("{openShiftChangeRequestId}")
    .decline(ScheduleChangeRequestDeclineParameterSet
        .newBuilder()
        .withMessage(message)
        .build())
    .buildRequest()
    .post();

```