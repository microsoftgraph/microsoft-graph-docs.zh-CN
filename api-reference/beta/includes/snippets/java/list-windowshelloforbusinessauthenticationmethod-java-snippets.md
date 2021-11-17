---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1b562ec4d64a81786233da058827e0e02334080b76d05b35736a3218e084008
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220169"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsHelloForBusinessAuthenticationMethodCollectionPage windowsHelloForBusinessMethods = graphClient.users("annie@contoso.com").authentication().windowsHelloForBusinessMethods()
    .buildRequest()
    .get();

```