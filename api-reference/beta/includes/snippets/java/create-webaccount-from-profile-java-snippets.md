---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3818ca15a7b9b029579708305a9718ab4326033
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969075"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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