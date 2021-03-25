---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb9695f3d1f49f40644be4ab11bd0856542a4148
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

KeyCredential keyCredential = new KeyCredential();
keyCredential.type = "AsymmetricX509Cert";
keyCredential.usage = "Verify";
keyCredential.key = Base64.getDecoder().decode("MIIDYDCCAki...");



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