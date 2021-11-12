---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e1af4f606c0aaeaf3a48ec343e32675ad1f23988312b940c0a7670126dec7e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903315"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionWithReferencesPage recentPlans = graphClient.me().planner().recentPlans()
    .buildRequest()
    .get();

```