---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dded8af787574c47572b1d09750fbd14677339c3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211068"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean _boolean = graphClient.teams("{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}").channels("19:33b76eea88574bd1969dca37e2b7a819@thread.skype")
    .doesUserHaveAccess(ChannelDoesUserHaveAccessParameterSet
        .newBuilder()
        .withUserId("62855810-484b-4823-9e01-60667f8b12ae")
        .withTenantId("57fb72d0-d811-46f4-8947-305e6072eaa5")
        .build())
    .buildRequest()
    .get();

```