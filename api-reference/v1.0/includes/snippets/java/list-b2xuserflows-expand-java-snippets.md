---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1110609866792867a1cdd9f9f344b3e1211c149ab82a86c04011c6398d64dfab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlowCollectionPage b2xUserFlows = graphClient.identity().b2xUserFlows()
    .buildRequest()
    .expand("identityProviders")
    .get();

```