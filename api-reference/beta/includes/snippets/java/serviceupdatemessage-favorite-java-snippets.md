---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c83cae7c56056f60d86c058e90c5fffe5e9f94cb8ac54690ecbc5c64eac28598
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903295"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> messageIdsList = new LinkedList<String>();
messageIdsList.add("MC172851");
messageIdsList.add("MC167983");

graphClient.admin().serviceAnnouncement().messages()
    .favorite(ServiceUpdateMessageFavoriteParameterSet
        .newBuilder()
        .withMessageIds(messageIdsList)
        .build())
    .buildRequest()
    .post();

```