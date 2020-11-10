---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51f2a0399f5fb17d2d2a17daf835f297c13c1c3d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957378"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConnectorCollectionPage members = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").members()
    .buildRequest()
    .get();

```