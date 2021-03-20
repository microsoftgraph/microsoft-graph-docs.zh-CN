---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e42878f25206231dfcde1964f76a25ac9dde0115
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976103"
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