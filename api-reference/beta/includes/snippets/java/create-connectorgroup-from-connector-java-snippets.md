---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffafd54e3862ac08151abc8f9a5bdb62a65104bbf216c883fcbef3b22b5a0696
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"));

graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}").memberOf().references()
    .buildRequest()
    .post(connectorGroup);

```