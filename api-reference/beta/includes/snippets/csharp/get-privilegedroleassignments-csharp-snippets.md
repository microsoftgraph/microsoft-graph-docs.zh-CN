---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 61e13366021151d86824b311afadc05b4b676321
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignments = await graphClient.PrivilegedRoleAssignments
    .Request()
    .Filter("isElevated eq true and expirationDateTime ne null or isElevated eq false")
    .GetAsync();

```