---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 41353698eaaa343f4786e61592fd02fd6585eeb3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890052"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerGroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```