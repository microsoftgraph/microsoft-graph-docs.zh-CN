---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e4b11bd02623e28a31b96a56624526d926c669d8e4fa1929ad1e1b9e12a3de2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryAudit = await graphClient.AuditLogs.DirectoryAudits["{directoryAudit-id}"]
    .Request()
    .GetAsync();

```