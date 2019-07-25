---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 105b667e4418da90400c1d5af00ab4425181c5b8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875468"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSummary privilegedRoleSummary = graphClient.privilegedRoles("{id}").summary()
    .buildRequest()
    .get();

```