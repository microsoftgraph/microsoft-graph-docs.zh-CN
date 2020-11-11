---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f78a657a602b990667e62df6fb454a6d54b3433b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983645"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.changeType = "created";
subscription.notificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient";
subscription.resource = "me/mailFolders('Inbox')/messages";
subscription.expirationDateTime = CalendarSerializer.deserialize("2016-11-20T18:23:45.9356913Z");
subscription.clientState = "secretClientValue";
subscription.latestSupportedTlsVersion = "v1_2";

graphClient.subscriptions()
    .buildRequest()
    .post(subscription);

```