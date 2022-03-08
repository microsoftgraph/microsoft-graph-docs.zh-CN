---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5be0b922b624806e69931fdadc422a942a3696cb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351207"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesAgentGroup onPremisesAgentGroup = graphClient.onPremisesPublishingProfiles("provisioning").agentGroups("2d55ed41-1619-4848-92bb-0576d3038682")
    .buildRequest()
    .expand("publishedResources,agents")
    .get();

```