---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5bcb612aab58960642f4ee915b5f19ab515b7d8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021420"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("Apple-Managed-OIDC")
    .buildRequest()
    .get();

```