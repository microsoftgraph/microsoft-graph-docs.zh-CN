---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40026a49f4cdafe6860e4d1005f1dbda060c34ff
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580595"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("MSASignup-OAUTH")
    .buildRequest()
    .get();

```