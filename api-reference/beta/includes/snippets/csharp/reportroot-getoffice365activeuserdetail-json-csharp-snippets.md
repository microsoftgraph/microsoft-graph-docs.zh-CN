---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 878887f0e6449e44ba12cda7315d25058c27f02c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActiveUserDetail = await graphClient.Reports
    .GetOffice365ActiveUserDetail('D7')
    .Request()
    .GetAsync();

```