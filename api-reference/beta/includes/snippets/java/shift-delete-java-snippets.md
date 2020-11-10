---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b1b49d84a9ae9031cd67a23fa5dc40050c41c2a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969196"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().shifts("{shiftId}")
    .buildRequest()
    .delete();

```