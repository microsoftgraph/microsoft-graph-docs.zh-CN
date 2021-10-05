---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0856e3a7432ddb98a6d13384a1c3c684b57b1014f04bd9b2938820cdef944690
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215956"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.changeType = "created";
subscription.notificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient";
subscription.resource = "me/mailFolders('Inbox')/messages";
subscription.expirationDateTime = OffsetDateTimeSerializer.deserialize("2016-11-20T18:23:45.9356913Z");
subscription.clientState = "secretClientValue";
subscription.latestSupportedTlsVersion = "v1_2";

graphClient.subscriptions()
    .buildRequest()
    .post(subscription);

```