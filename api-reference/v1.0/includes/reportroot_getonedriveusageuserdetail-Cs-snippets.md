---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 259598fe4725008d1ddc42e28ac70eb978e0e96c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveUsageAccountDetail('D7')
    .Request()
    .GetAsync();

```