---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efa92f06ad34a0c7a37a5bb4f906e15733797e4c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968454"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnniversary personAnniversary = graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .get();

```