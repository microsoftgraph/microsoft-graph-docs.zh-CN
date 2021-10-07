---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8428a2fc291ede6b60a9ec5d99d01dd6386dbc74
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214788"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChannelGetAllMessagesCollectionPage getAllMessages = graphClient.teams("01fe12e0-e720-44fd-8854-28c66d1bee40").channels()
    .getAllMessages()
    .buildRequest()
    .filter("lastModifiedDateTime gt 2019-11-01T00:00:00Z and lastModifiedDateTime lt 2021-11-01T00:00:00Z")
    .get();

```