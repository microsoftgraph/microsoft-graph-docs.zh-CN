---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3787aefa6105b9840929432c5a10c99f6d699691
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"));

graphClient.identity().b2xUserFlows("B2X_1_testuserflow").postFederationSignup().reference()
    .buildRequest()
    .put(identityApiConnector);

```