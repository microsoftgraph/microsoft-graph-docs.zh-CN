---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98c14343a9327318f9254e6f180327969504a65680d7679e8a3b3c448808e14f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278951"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("Apple-Managed-OIDC")
    .buildRequest()
    .get();

```