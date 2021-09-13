---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24c0ca96ae17b59e4e5dba00b9e3ea2faf2edfbe524cbc068920fe9e0f8f80f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106031"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().plans("{plan-id}").tasks()
    .buildRequest()
    .get();

```