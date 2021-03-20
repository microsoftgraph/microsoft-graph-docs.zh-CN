---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f41224ecee778f41106db17896ce08ce16f95c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973245"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = new WebAccount();
webAccount.webUrl = "https://github.com/innocenty.popov";

graphClient.me().profile().webAccounts("{id}")
    .buildRequest()
    .patch(webAccount);

```