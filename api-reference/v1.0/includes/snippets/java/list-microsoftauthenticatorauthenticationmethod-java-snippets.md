---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fadba5a946d4ea567f8b0f67dd3e5f17ad8c86268513968b01ae05b78ed31be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218749"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethodCollectionPage microsoftAuthenticatorMethods = graphClient.users("sandeep@contoso.com").authentication().microsoftAuthenticatorMethods()
    .buildRequest()
    .get();

```