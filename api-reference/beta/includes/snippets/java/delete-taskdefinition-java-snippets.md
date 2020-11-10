---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6be9202cf988af72e7c35e08e0c82fb0ed332dcb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967111"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().taskDefinitions("4c6a0f26-8e5d-4bf6-91e6-4a5731adec19")
    .buildRequest()
    .delete();

```