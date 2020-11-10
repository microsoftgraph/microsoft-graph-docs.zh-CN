---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9af667b46037bc313bb7dd74b19000ec574d042
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964882"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .resetUnseenCount()
    .buildRequest()
    .post();

```