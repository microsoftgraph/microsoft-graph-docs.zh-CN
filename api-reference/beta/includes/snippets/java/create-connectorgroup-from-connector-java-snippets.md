---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72332ff8124a67841c1cce5373dadff717a041ba
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753003"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"));

graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}").memberOf().references()
    .buildRequest()
    .post(connectorGroup);

```