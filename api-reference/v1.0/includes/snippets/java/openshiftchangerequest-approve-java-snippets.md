---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e01de0e87f5a8b4fbb49c0c48060bd31726914b795d379e2f5a2d5a5582c631
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107003"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "message-value";

graphClient.teams("{id}").schedule().openShiftChangeRequests("{openShiftChangeRequestId}")
    .approve(ScheduleChangeRequestApproveParameterSet
        .newBuilder()
        .withMessage(message)
        .build())
    .buildRequest()
    .post();

```