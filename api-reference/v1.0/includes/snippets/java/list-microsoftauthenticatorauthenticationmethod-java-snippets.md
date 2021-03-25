---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 151ed3a1ff220420c5c0290c0d8be26f2aed133d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202566"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethodCollectionPage microsoftAuthenticatorMethods = graphClient.users("sandeep@contoso.com").authentication().microsoftAuthenticatorMethods()
    .buildRequest()
    .get();

```