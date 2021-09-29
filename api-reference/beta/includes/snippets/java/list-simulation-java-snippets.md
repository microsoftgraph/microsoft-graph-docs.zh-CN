---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 472ead3753692cc588e8b685cd8338964c36d042
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995973"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SimulationCollectionPage simulations = graphClient.security().attackSimulation().simulations()
    .buildRequest()
    .get();

```