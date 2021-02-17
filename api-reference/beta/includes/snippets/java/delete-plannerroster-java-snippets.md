---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55adb4596e3bc4fd852e4df8995e002858b38b15
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271929"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.planner().rosters("5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38")
    .buildRequest()
    .delete();

```