---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5c6c5839fbae6418a67240fd62c41d8c61d44fa9d2954142f8f303960ce9339
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409698"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").progressTaskBoardFormat()
    .buildRequest()
    .get();

```