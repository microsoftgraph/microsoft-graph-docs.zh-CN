---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cfe22e6d4b86297f7da34d7176f650994d7269f48faf77af27b64247b91c753
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220794"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationMethodConfiguration authenticationMethodConfiguration = graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("passwordlessMicrosoftAuthenticator")
    .buildRequest()
    .get();

```