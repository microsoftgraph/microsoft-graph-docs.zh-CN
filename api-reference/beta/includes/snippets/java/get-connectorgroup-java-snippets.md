---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bb6808c026a6b5c2586418cc983a333b803d61f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}")
    .buildRequest()
    .get();

```