---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75d65b1717eb7d75b286e4bcce002216d40b9827
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953304"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().userFlows("{id}")
    .buildRequest()
    .delete();

```