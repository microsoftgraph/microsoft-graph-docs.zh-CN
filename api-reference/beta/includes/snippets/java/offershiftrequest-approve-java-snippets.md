---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fa0666bca077f65a9543b408926ae329c92e505
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969742"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "Approved!";

graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .approve(ScheduleChangeRequestApproveParameterSet
        .newBuilder()
        .withMessage(message)
        .build())
    .buildRequest()
    .post();

```