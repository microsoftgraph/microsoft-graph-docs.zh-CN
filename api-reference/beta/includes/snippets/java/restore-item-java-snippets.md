---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d6a9758eff7d488a5d07faf82aa3636985a73b7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963527"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference parentReference = new ItemReference();
parentReference.id = "String";

String name = "String";

graphClient.me().drive().items("{item-id}")
    .restore(parentReference,name)
    .buildRequest()
    .post();

```