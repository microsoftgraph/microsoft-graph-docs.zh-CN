---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0893c31c1614fe0422caf92c31c4964b82326059
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972648"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = new WebAccount();
webAccount.description = "My Github contributions!";
webAccount.userId = "innocenty.popov";
ServiceInformation service = new ServiceInformation();
service.name = "GitHub";
service.webUrl = "https://github.com";
webAccount.service = service;

graphClient.me().profile().webAccounts()
    .buildRequest()
    .post(webAccount);

```