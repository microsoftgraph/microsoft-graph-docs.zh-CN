---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 867b75745141fc4b570f35b3e8703301af39863a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970377"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoles("{id}")
    .selfDeactivate()
    .buildRequest()
    .post();

```