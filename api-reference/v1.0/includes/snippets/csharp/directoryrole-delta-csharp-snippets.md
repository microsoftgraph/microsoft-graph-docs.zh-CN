---
description: 自动生成的文件。 不修改
ms.openlocfilehash: afc31a36c4e0a89a0f3151a6a1328f19b0d17381
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.DirectoryRoles
    .Delta()
    .Request()
    .GetAsync();

```