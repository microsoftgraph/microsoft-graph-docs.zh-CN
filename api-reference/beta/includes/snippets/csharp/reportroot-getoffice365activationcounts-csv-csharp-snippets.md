---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b010ffd8ae307f4f69d06f8882ad6990db1a5a3e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationCounts = await graphClient.Reports
    .GetOffice365ActivationCounts()
    .Request()
    .GetAsync();

```