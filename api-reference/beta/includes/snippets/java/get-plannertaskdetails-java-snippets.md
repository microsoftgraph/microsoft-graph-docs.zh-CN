---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d891ab9ade9615cefd383f3cf14162ddac92e54a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876237"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskDetails plannerTaskDetails = graphClient.planner().tasks("gcrYAaAkgU2EQUvpkNNXLGQAGTtu").details()
    .buildRequest()
    .get();

```