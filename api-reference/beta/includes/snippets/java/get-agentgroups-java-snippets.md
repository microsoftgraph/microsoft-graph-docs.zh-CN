---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2f73f3bd501c58938834b044237cae640f7d3b23
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878385"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnPremisesAgentGroupCollectionPage agentGroups = graphClient.onPremisesPublishingProfiles("provisioning").agentGroups()
    .buildRequest()
    .expand("publishedResources")
    .get();

```