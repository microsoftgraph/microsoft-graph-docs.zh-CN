---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b17055958e6df714b1fc69690357ff3c9e55beba
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208748"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

KeyCredential keyCredential = new KeyCredential();
keyCredential.type = "X509CertAndPassword";
keyCredential.usage = "Sign";
keyCredential.key = Base64.getDecoder().decode("MIIDYDCCAki...");

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.secretText = "MKTr0w1...";

String proof = "eyJ0eXAiOiJ...";

graphClient.applications("{id}")
    .addKey(ApplicationAddKeyParameterSet
        .newBuilder()
        .withKeyCredential(keyCredential)
        .withPasswordCredential(passwordCredential)
        .withProof(proof)
        .build())
    .buildRequest()
    .post();

```