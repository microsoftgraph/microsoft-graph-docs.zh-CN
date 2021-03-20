---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d04efbe19c55fa381fc72e0f020071a81b7ccc87
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977092"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().plans("xqQg5FS2LkCp935s-FIFm2QAFkHM").tasks()
    .buildRequest()
    .get();

```