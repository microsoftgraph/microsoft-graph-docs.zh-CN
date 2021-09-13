---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2077b8b6b85b3962a1725becf10025857872b207466127cc8148355aa643984
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218703"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").bucketTaskBoardFormat()
    .buildRequest()
    .get();

```