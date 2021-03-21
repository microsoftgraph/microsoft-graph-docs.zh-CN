---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78e99f1f73a3b14e2aa35a945f9d01f78bb133da
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984233"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTask plannerTask = graphClient.planner().tasks("01gzSlKkIUSUl6DF_EilrmQAKDhh")
    .buildRequest()
    .get();

```