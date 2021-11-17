---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72da09aa173450e49d34dcaec83ac800762f58563a8a22654399b62c830a5738
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220791"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerDeltaDeltaCollectionPage delta = graphClient.me().planner().all()
    .delta()
    .buildRequest()
    .get();

```