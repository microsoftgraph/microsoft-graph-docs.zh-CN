---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c90c154f25e1b46a45a097bf96dc9ccea01f661e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957946"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .delete();

```