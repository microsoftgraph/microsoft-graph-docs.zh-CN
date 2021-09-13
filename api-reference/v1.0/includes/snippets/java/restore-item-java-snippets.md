---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86f9603f475cd596bf2aa1b6f4ce92151f70df01d6c22f15344ddb2fcf131857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409084"
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