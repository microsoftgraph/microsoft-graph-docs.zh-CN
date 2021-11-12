---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3debb7697fff7daf79fc21bf9f188001c7929c290a45d90ccdf3c4816fd8c570
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902511"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.name = "name-value";
connectorGroup.isDefault = false;

graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups()
    .buildRequest()
    .post(connectorGroup);

```