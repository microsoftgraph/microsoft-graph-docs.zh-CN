---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c2b374828026eadfa2bc6904315175f38108811
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975909"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/apiConnectors/{id}"));

graphClient.identity().b2xUserFlows("B2X_1_testuserflow").postFederationSignup().reference()
    .buildRequest()
    .put(identityApiConnector);

```