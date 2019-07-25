---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25c3f9dd496c2a2bb6eee627a0d0b5b8b9788ca0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731191"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var licenseDetails = await graphClient.Me.LicenseDetails
    .Request()
    .GetAsync();

```