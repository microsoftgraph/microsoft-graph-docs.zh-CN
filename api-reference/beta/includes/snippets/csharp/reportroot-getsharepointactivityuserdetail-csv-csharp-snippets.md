---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 626292d81cb143bb580bcc350bcd10d082d11229
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointActivityUserDetail = await graphClient.Reports
    .GetSharePointActivityUserDetail('D7')
    .Request()
    .GetAsync();

```