---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d4ca9204d24841dd073013255d554f94def1a3e3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignments
    .My()
    .Request()
    .GetAsync();

```