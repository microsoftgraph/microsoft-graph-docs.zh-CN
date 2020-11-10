---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49a8516ed82d085dfc2fbefe80847b8c238fa4e0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954159"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest()
    .get();

```