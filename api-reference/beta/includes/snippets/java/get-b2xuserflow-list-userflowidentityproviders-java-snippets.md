---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 838e5ffadfe01c1f54f4c67d9a832c1fcc762f35
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439605"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseCollectionWithReferencesPage userFlowIdentityProviders = graphClient.identity().b2xUserFlows("B2X_1_Test").userFlowIdentityProviders()
    .buildRequest()
    .get();

```