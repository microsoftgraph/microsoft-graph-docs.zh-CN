---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79ff03fa3840438d5c7c1e795816929d952d49ed26e49710a36192b18481beea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163377"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionWithReferencesPage favoritePlans = graphClient.me().planner().favoritePlans()
    .buildRequest()
    .get();

```