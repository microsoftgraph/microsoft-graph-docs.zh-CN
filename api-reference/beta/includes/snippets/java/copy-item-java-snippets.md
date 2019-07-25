---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 618fab482484ea87994f4193c873fe4dadbc1cec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861382"
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