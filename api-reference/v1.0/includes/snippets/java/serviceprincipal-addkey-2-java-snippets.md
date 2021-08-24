---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2808c83beadc469ef869ffa2989d09d601ba22405a401d4b9fa9e29fdc690a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334083"
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