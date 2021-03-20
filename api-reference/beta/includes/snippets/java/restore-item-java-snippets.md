---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cab0cd5c858a90f497f548f4af348e67d91bec91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967997"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference parentReference = new ItemReference();
parentReference.id = "String";

String name = "String";

graphClient.me().drive().items("{item-id}")
    .restore(DriveItemRestoreParameterSet
        .newBuilder()
        .withParentReference(parentReference)
        .withName(name)
        .build())
    .buildRequest()
    .post();

```