---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9b0640b0d83e2a795fbfb7d1119bb3a4bcae8d0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212812"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> requestIdsList = new LinkedList<String>();
requestIdsList.add("f01c6af6-6683-4a37-a945-0a925501eede");
requestIdsList.add("42bf60ac-d0cb-4206-aa5c-101884298f55");
requestIdsList.add("f09c8f14-8d8e-42cf-8a7e-732b0594e79b");

graphClient.auditLogs().signIns()
    .confirmCompromised(SignInConfirmCompromisedParameterSet
        .newBuilder()
        .withRequestIds(requestIdsList)
        .build())
    .buildRequest()
    .post();

```