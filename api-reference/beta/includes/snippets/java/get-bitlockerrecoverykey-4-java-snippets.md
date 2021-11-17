---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b84c00563ae92b795dea59aecbd5000a236e9239db8945292bf214732a8b37d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105860"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BitlockerRecoveryKey bitlockerRecoveryKey = graphClient.informationProtection().bitlocker().recoveryKeys("b465e4e8-e4e8-b465-e8e4-65b4e8e465b4")
    .buildRequest()
    .select("key")
    .get();

```