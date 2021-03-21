---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13de7a1f7d41fbbd8237d2715919c3a1da24fe3e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983522"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethod microsoftAuthenticatorAuthenticationMethod = graphClient.users("anirban@contoso.com").authentication().microsoftAuthenticatorMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .get();

```