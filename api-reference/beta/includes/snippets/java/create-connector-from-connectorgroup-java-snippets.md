---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7127663f314477d3e8bb7442ae46c13e6a7ec37ada27601834f376673b978c29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101409"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Connector connector = new Connector();
connector.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"));

graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").members().references()
    .buildRequest()
    .post(connector);

```