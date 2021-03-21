---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7949ce8386346683fb33b8b1dfb1b1167a6bbcc7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974881"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").progressTaskBoardFormat()
    .buildRequest()
    .get();

```