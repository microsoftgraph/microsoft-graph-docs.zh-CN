---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0aca4092782d56d8e206ee3060d0bd0f6786f8de5174286ec94292e8140be72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332333"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().tasks()
    .buildRequest()
    .get();

```