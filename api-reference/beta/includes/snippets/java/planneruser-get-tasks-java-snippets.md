---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8a37c5d50f7b9a318b734d6a061c4044418fca31775e517242fc09f2010601d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328916"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.me().planner().tasks()
    .buildRequest()
    .get();

```