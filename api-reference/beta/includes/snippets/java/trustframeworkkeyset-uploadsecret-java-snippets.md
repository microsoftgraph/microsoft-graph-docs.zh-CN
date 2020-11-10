---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 881072d99366d4c1be509d24237d93a0a735628c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972171"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String use = "use-value";

String k = "application-secret-to-be-uploaded";

Long nbf = 1508969811L;

Long exp = 1508973711L;

graphClient.trustFramework().keySets("{id}")
    .uploadSecret(use,k,nbf,exp)
    .buildRequest()
    .post();

```