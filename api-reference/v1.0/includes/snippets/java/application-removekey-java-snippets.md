---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef174c14b2ccabcedbe2f50f8434d9135ade8e5fe14e3c4b86328142ad05af3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101345"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID keyId = UUID.fromString("f0b0b335-1d71-4883-8f98-567911bfdca6");

String proof = "eyJ0eXAiOiJ...";

graphClient.applications("{id}")
    .removeKey(ApplicationRemoveKeyParameterSet
        .newBuilder()
        .withKeyId(keyId)
        .withProof(proof)
        .build())
    .buildRequest()
    .post();

```