---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 09d10529ef5e2287a8ee30a30a3b4ec14cf02426
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var auditLogRoot = await graphClient.AuditLogs
    .Request()
    .GetAsync();

```