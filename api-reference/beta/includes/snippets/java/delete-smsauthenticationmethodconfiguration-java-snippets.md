---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f7a7d1686d7a3310ae90623f7c3f93e7f6a9b5775607f3e21713d1134cc3bda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279466"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("sms")
    .buildRequest()
    .delete();

```