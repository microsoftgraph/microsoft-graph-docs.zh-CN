---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c8db06b901d7d2cc5c690bdd4c2b9f035598e2eb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875066"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPublishedResourceCollectionPage publishedResources = graphClient.onPremisesPublishingProfiles("{publishingType}").publishedResources()
    .buildRequest()
    .expand("agentGroups")
    .get();

```