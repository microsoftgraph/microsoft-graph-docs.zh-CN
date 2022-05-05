---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63329d5237d9f26c271d698d940ea8f794dd1951
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209248"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("ece6f0a1-7ca4-498b-be79-edf6c8fc4d82").incomingChannels("19:56eb04e133944cf69e603c5dac2d292e@thread.skype").reference()
    .buildRequest()
    .delete();

```