---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8decb00c9c96188936a22d4da727128dd2acba99
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881048"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActivationsUserDetail()
    .Request()
    .GetAsync();

```