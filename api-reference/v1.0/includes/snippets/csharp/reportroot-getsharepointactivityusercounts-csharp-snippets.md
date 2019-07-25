---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1fc6dc4c1bf0eb2e7162b4c6e49ca952466d0a11
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893523"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSharePointActivityUserCounts('D7')
    .Request()
    .GetAsync();

```