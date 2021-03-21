---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03f5749fbe4ba726c2ca567f36a734620f2633f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978711"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskDetails plannerTaskDetails = graphClient.planner().tasks("{task-id}").details()
    .buildRequest()
    .get();

```