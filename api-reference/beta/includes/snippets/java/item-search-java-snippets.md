---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cbd5a6d6d500806878e3cd213211522b8d26848
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975842"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemSearchCollectionPage search = graphClient.me().drive().root()
    .search(DriveItemSearchParameterSet
        .newBuilder()
        .withQ("Contoso Project")
        .build())
    .buildRequest()
    .get();

```