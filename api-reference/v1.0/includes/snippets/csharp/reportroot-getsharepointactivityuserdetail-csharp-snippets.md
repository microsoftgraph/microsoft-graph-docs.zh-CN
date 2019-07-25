---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 081f6a257f83365e9e20e6d8fab38cff35426e79
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityUserDetail('D7')
    .Request()
    .GetAsync();

```