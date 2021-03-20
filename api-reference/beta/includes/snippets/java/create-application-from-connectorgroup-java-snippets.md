---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80ae48b186b1ebf84750d3679834bf95aa2d521d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975355"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"));

graphClient.applications("{id}").connectorGroup().reference()
    .buildRequest()
    .put(connectorGroup);

```