---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6fe73181843375f86be254b25f4d30ab66156e1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996666"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSimulationDetailsCollectionPage simulationUsers = graphClient.customRequest("/security/attackSimulation/simulations/{id}/report/simulationUsers", UserSimulationDetailsCollectionPage.class)
    .buildRequest()
    .get();

```