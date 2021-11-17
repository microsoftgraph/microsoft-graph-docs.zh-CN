---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49c103b3cc731a8f31b8b1948e528ad2c6719849e0c5d8b097ebb8a62863bc48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219599"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .unmute(CallUnmuteParameterSet
        .newBuilder()
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```