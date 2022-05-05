---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 495813b7536b740bfcdcc04f6ab7690ddcf8d3fd
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210450"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "785f4929-92ca-497b-863f-c778c77c9758";

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .addLargeGalleryView(CallAddLargeGalleryViewParameterSet
        .newBuilder()
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```