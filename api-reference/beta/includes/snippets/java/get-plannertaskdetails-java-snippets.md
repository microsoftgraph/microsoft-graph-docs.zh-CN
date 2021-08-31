---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3b326d93cfe547297fa8c4876789c7966915939f3590813a5e3918779b5af68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105728"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskDetails plannerTaskDetails = graphClient.planner().tasks("gcrYAaAkgU2EQUvpkNNXLGQAGTtu").details()
    .buildRequest()
    .get();

```