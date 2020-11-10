---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c67d8fa8713ba604ccda0925083d6f3751bc20d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961197"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2cUserFlows("{id}").identityProviders()
    .buildRequest()
    .get();

```