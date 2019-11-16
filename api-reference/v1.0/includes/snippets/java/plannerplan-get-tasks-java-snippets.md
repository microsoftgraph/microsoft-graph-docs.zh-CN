---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f850bf51d98ebf7b3cf64481ddfde0b92cfba0c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637835"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerTaskCollectionPage tasks = graphClient.planner().plans("{plan-id}").tasks()
    .buildRequest()
    .get();

```