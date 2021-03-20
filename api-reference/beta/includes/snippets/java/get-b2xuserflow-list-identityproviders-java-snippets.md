---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71be43d9fc37679ba8c0a6f31dc21c1544aba1f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975289"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2xUserFlows("{id}").identityProviders()
    .buildRequest()
    .get();

```