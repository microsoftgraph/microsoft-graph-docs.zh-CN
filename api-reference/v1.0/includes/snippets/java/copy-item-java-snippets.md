---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 780b116f8d5b380609b4d1a28b3491ce88dfd2025e684a1657ab711456575ff8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333518"
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