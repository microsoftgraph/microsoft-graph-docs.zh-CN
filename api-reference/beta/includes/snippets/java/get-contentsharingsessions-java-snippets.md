---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cfebbce2702bddcc454208e778fd01b048afb6d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211610"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentSharingSessionCollectionPage contentSharingSessions = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").contentSharingSessions()
    .buildRequest()
    .get();

```