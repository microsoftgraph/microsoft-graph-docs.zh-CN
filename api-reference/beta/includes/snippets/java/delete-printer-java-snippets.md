---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e064422621fb6c8c95c24e1ff469a84a2996f8ab
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981479"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}")
    .buildRequest()
    .delete();

```