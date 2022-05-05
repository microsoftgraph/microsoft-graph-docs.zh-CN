---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8686a1bde1162bc86107e54279ce9c86d6ab39c1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203613"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SimulationAutomationCollectionPage simulationAutomations = graphClient.security().attackSimulation().simulationAutomations()
    .buildRequest()
    .get();

```