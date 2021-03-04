---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ac4bd9166afd496cf91e6a19671bd7d9c880313
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433373"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWindowsHelloForBusinessAuthenticationMethodCollectionPage windowsHelloForBusinessMethods = graphClient.users("annie@contoso.com").authentication().windowsHelloForBusinessMethods()
    .buildRequest()
    .get();

```