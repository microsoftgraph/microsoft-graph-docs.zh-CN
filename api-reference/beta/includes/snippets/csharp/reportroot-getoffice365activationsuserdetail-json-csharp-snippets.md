---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7ffb1d3678ade75070a5e3c6114867d38324e90e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873511"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365ActivationsUserDetail = await graphClient.Reports
    .GetOffice365ActivationsUserDetail()
    .Request()
    .GetAsync();

```