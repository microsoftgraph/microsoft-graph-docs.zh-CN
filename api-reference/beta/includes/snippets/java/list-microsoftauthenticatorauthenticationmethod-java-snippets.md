---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c209fd0a61dac54124162e39f007b68bb1c924a89a3a85bbfd483eeaf8aa063
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273986"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethodCollectionPage microsoftAuthenticatorMethods = graphClient.users("anirban@contoso.com").authentication().microsoftAuthenticatorMethods()
    .buildRequest()
    .get();

```