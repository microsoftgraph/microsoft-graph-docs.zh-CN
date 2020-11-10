---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41b46a1e474bf9fe670c79eddf30e3461d918f12
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970730"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkforceIntegration workforceIntegration = graphClient.teamwork().workforceIntegrations("{workforceintegrationid}")
    .buildRequest()
    .get();

```