---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 971baa1c3aaf52067106aa9091329b8f52adf8d4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439653"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2C_test_signin_signup").userFlowIdentityProviders("MSA-OIDC").reference()
    .buildRequest()
    .delete();

```