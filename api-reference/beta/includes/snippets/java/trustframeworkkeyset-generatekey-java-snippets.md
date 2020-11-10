---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67478c5e2447ad4bbd84945cb4f3adf1b1a1db0d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981684"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String use = "sig";

String kty = "RSA";

Long nbf = 1508969811L;

Long exp = 1508969811L;

graphClient.trustFramework().keySets("{id}")
    .generateKey(use,kty,nbf,exp)
    .buildRequest()
    .post();

```