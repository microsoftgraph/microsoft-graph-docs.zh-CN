---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 118ea4a87d1c4c75f831c58cb0e1c99c4c6480e0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964857"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .unsubscribeByMail()
    .buildRequest()
    .post();

```