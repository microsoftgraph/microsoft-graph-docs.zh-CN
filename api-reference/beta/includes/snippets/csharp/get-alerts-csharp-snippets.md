---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7bf07cb98320e2f06b14a844161a67289bb8ffff
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alerts = await graphClient.Security.Alerts
    .Request()
    .GetAsync();

```