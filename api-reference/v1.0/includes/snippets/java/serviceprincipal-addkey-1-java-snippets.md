---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f59dcbe300177b8a7328e68b416b86f611f55e217ba3bd9da656f0160dcd6f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334084"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

KeyCredential keyCredential = new KeyCredential();
keyCredential.type = "AsymmetricX509Cert";
keyCredential.usage = "Verify";
keyCredential.key = Base64.getDecoder().decode("MIIDYDCCAki...");



String proof = "eyJ0eXAiOiJ...";

graphClient.servicePrincipals("{id}")
    .addKey(ServicePrincipalAddKeyParameterSet
        .newBuilder()
        .withKeyCredential(keyCredential)
        .withPasswordCredential(passwordCredential)
        .withProof(proof)
        .build())
    .buildRequest()
    .post();

```