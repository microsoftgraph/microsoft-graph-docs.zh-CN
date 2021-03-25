---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eafca69cd7cc3051b0f306b05cdd204023de924a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208402"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BitlockerRecoveryKey bitlockerRecoveryKey = graphClient.informationProtection().bitlocker().recoveryKeys("b465e4e8-e4e8-b465-e8e4-65b4e8e465b4")
    .buildRequest()
    .select("key")
    .get();

```