---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 262d48f2a211a69dc507867ce7d10275092cca89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977480"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlowCollectionPage b2cUserFlows = graphClient.identity().b2cUserFlows()
    .buildRequest()
    .expand("identityProviders")
    .get();

```