---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 075b7ee29fb67da1858905bac5b699e9ad096d84ab90d76b337e83bdb4308e6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328811"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroupCollectionPage memberOf = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}").memberOf()
    .buildRequest()
    .get();

```