---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32c9c758f2e9966058251aae4b7ec2a95c2bda69
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "Sorry, you can't offer this shift.";

graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .decline(message)
    .buildRequest()
    .post();

```