---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 606781b9feebdf89e3eca136900674c7e1b1f6f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966738"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethodCollectionPage microsoftAuthenticatorMethods = graphClient.users("anirban@contoso.com").authentication().microsoftAuthenticatorMethods()
    .buildRequest()
    .get();

```