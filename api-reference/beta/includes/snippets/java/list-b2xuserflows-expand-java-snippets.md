---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63359eb997c7a4928b9f468e8099acc4aa4dae48
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953550"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IB2xIdentityUserFlowCollectionPage b2xUserFlows = graphClient.identity().b2xUserFlows()
    .buildRequest()
    .expand("identityProviders")
    .get();

```