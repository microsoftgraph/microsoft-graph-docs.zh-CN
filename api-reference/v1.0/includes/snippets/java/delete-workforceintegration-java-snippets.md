---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a93f12865dea16cf5c3997159c61df4957e51a3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217279"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teamwork().workforceIntegrations("{workforceIntegrationId}")
    .buildRequest()
    .delete();

```