---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ab2544b4807cbb06d0666221a1e1dcc2f8c65f2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980778"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference parentReference = new ItemReference();
parentReference.driveId = "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B";
parentReference.id = "DCD0D3AD-8989-4F23-A5A2-2C086050513F";

String name = "contoso plan (copy).txt";

graphClient.me().drive().items("{item-id}")
    .copy(DriveItemCopyParameterSet
        .newBuilder()
        .withName(name)
        .withParentReference(parentReference)
        .build())
    .buildRequest()
    .post();

```