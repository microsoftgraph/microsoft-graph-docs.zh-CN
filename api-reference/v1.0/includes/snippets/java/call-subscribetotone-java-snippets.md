---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7897ff7742e6cb226e4dce09c0b2ecca2a4284f30d4c43bb92fe12dd92e837b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334003"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54";

graphClient.communications().calls("{id}")
    .subscribeToTone(CallSubscribeToToneParameterSet
        .newBuilder()
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```