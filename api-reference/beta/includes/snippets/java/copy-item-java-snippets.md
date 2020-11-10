---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 618fab482484ea87994f4193c873fe4dadbc1cec
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955681"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference parentReference = new ItemReference();
parentReference.driveId = "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B";
parentReference.id = "DCD0D3AD-8989-4F23-A5A2-2C086050513F";

String name = "contoso plan (copy).txt";

graphClient.me().drive().items("{item-id}")
    .copy(name,parentReference)
    .buildRequest()
    .post();

```