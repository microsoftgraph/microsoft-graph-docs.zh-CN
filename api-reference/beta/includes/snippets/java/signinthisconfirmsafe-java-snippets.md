---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e1f0dbd07a29c3a3dd843dc397a57e139880a60
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212743"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> requestIdsList = new LinkedList<String>();
requestIdsList.add("5a0c76d2-cb57-4ece-9bc1-c323178f116a");
requestIdsList.add("96609214-09ef-4f80-9d4a-ace5fceecaec");
requestIdsList.add("05020696-4eb8-45a3-918f-8f8bb7ad6015");

graphClient.auditLogs().signIns()
    .confirmSafe(SignInConfirmSafeParameterSet
        .newBuilder()
        .withRequestIds(requestIdsList)
        .build())
    .buildRequest()
    .post();

```