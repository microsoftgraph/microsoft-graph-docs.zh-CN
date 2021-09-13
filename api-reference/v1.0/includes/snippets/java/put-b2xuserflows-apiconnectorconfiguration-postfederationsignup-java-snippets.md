---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2d90105a5004eebaf7a269b1543847d0638d1a91acfce8469990b5aea615416
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105418"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"));

graphClient.identity().b2xUserFlows("B2X_1_testuserflow").postFederationSignup().reference()
    .buildRequest()
    .put(identityApiConnector);

```