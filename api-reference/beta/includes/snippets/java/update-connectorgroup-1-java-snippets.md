---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6664c926fed3663aa6b826abd9b1f58c21d08b9f125a3cdcb6d49613469dbf72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101407"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.name = "Connector Group Demo";

graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups()
    .buildRequest()
    .post(connectorGroup);

```