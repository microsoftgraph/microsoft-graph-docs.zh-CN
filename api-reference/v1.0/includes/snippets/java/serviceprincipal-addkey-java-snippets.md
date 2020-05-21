---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b4aa24bd09ec280b4ece349619f7e9715a19c4b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334448"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

KeyCredential keyCredential = new KeyCredential();
keyCredential.type = "X509CertAndPassword";
keyCredential.usage = "Sign";
keyCredential.key = "MIIDYDCCAki...";

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.secretText = "MKTr0w1...";

String proof = "eyJ0eXAiOiJ...";

graphClient.serviceprincipals("{id}")
    .addKey(keyCredential,passwordCredential,proof)
    .buildRequest()
    .post();

```