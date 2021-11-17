---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ada4ce7da7a641dea0ccf5973787e8f49a74d8dcfafdfcd726fd726bde337451
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219117"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRoster plannerRoster = graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965")
    .buildRequest()
    .get();

```