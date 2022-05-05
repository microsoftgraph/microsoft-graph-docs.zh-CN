---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d19385ac516a0d7497699d30eda2d6769d74ca5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIns = await graphClient.AuditLogs.SignIns
    .Request()
    .Filter("startsWith(appDisplayName,'Azure')")
    .Top(10)
    .GetAsync();

```