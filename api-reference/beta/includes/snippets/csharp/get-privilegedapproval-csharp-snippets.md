---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7256b6fab723f80774692c49c814fe9a74bf146f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval
    .Request()
    .GetAsync();

```