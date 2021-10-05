---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f05f9b25e706c45cc4275d3f1dea3b5b08b875e7d9fa819d23e2f1c4f261d982
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106220"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.expirationDateTime = OffsetDateTimeSerializer.deserialize("2016-11-22T18:23:45.9356913Z");

graphClient.subscriptions("{id}")
    .buildRequest()
    .patch(subscription);

```