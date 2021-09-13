---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96d52647c902ebe451c2245203b44295bba4e6ede95114075aee382bd2707d8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163483"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketCollectionPage buckets = graphClient.planner().plans("{plan-id}").buckets()
    .buildRequest()
    .get();

```