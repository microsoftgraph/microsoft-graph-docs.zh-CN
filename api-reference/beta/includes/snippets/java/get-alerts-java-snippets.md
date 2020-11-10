---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1889a652eb8c6029041095b818be4b9925decd45
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962382"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAlertCollectionPage alerts = graphClient.security().alerts()
    .buildRequest()
    .get();

```