---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbb7021603a2dca5c41225166ac911e2cce027d9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973418"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.onPremisesPublishingProfiles("provisioning").publishedResources("1234b780-965f-4149-85c5-a8c73e58b67d").agentGroups("8832388F-3814-4952-B288-FFB62081FE25").reference()
    .buildRequest()
    .delete();

```