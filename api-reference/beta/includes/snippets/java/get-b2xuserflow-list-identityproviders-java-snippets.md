---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ca9a0f38055ae432c948b1e5dc5902c0886bb91f0a2ea581db7abe36fc397eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105660"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2xUserFlows("{id}").identityProviders()
    .buildRequest()
    .get();

```