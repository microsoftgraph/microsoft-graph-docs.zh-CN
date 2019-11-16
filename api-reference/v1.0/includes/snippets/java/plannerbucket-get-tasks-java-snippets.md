---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b149cd9b63eacdee90e3ce8056b9300456f5553c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637863"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerTaskCollectionPage tasks = graphClient.planner().buckets("{task-id}").tasks()
    .buildRequest()
    .get();

```