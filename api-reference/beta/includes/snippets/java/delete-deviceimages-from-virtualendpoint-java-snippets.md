---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d844d994bb3021111fdff98ab33fcac067a409c
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521878"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().deviceImages("{id}")
    .buildRequest()
    .delete();

```