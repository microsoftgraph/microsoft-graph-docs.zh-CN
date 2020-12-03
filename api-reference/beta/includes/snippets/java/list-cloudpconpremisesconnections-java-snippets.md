---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 024fcb8cc44675cdba032fa44af0e98e0ec81cf8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522609"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICloudPcOnPremisesConnectionCollectionPage onPremisesConnections = graphClient.deviceManagement().virtualEndpoint().onPremisesConnections()
    .buildRequest()
    .get();

```