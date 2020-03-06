---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d57eadb6d8537440f253ce8f5fa5513c7bf7d56
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638117"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = false;

graphClient.contacts("{id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```