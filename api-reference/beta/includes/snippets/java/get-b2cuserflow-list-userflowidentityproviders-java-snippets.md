---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc199589d25e6679fab40e36ef798d069ab2ee4b09991a09da5c370dfbe6b808
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161935"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseCollectionWithReferencesPage userFlowIdentityProviders = graphClient.identity().b2cUserFlows("B2C_test_signin_signup").userFlowIdentityProviders()
    .buildRequest()
    .get();

```