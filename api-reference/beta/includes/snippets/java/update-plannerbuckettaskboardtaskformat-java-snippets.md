---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 883e12b539d7f781b932b3d73a4f1c7b858b547efabc4c92dcf62f181f809d78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218472"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = new PlannerBucketTaskBoardTaskFormat();
plannerBucketTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("hsOf2dhOJkqyYYZEtdzDe2QAIUCR").bucketTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerBucketTaskBoardTaskFormat);

```