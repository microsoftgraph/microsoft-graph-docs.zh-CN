---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c04e8533ec3656d86206a6d84dabb1e85004631
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209974"
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