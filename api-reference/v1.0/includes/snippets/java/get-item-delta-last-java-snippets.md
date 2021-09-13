---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2262b8a9b9a70184b6749834fbe14cf9ffe067cb96b5490fab778ca39c52bb85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902985"
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