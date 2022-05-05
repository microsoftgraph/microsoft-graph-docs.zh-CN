---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c6b3e3e2367281bdc37430316d12be64d1c70c7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InternalDomainFederation internalDomainFederation = new InternalDomainFederation();
internalDomainFederation.displayName = "Contoso name change";
internalDomainFederation.federatedIdpMfaBehavior = FederatedIdpMfaBehavior.ACCEPT_IF_MFA_DONE_BY_FEDERATED_IDP;

graphClient.domains("contoso.com").federationConfiguration("6601d14b-d113-8f64-fda2-9b5ddda18ecc")
    .buildRequest()
    .patch(internalDomainFederation);

```