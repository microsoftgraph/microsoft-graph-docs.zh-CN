---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 909bd71a21ada701fad2bdfe9d22a31e1398d25b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875903"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedApprovalCollectionPage myRequests = graphClient.privilegedApproval()
    .myRequests()
    .buildRequest()
    .get();

```