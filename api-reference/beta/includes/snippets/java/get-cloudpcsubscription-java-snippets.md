---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30622370775f30aa59b214b6be035cc2ac19f2bb
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629292"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcSnapshotGetSubscriptionsCollectionPage getSubscriptions = graphClient.deviceManagement().virtualEndpoint().snapshots()
    .getSubscriptions()
    .buildRequest()
    .get();

```