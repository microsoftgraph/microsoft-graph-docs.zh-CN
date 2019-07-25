---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cf1908605d7d9c38b12113413941ea0bf62017f1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871264"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerGroupsActivityGroupCounts = await graphClient.Reports
    .GetYammerGroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```