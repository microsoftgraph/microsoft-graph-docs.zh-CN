---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5a546b405bdd069e4da64d8091648f458e78e85
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982908"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.expirationDateTime = CalendarSerializer.deserialize("2016-11-22T18:23:45.9356913Z");

graphClient.subscriptions("{id}")
    .buildRequest()
    .patch(subscription);

```