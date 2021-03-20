---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fa2d054c054383934ccc3282e05eb3aa8841d09
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971249"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta(DriveItemDeltaParameterSet
        .newBuilder()
        .withToken("1230919asd190410jlka")
        .build())
    .buildRequest()
    .get();

```