---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 123c9a02fcc9bd4e58f730c86afd8e05af1106e7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439744"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseCollectionWithReferencesPage userFlowIdentityProviders = graphClient.identity().b2cUserFlows("B2C_test_signin_signup").userFlowIdentityProviders()
    .buildRequest()
    .get();

```