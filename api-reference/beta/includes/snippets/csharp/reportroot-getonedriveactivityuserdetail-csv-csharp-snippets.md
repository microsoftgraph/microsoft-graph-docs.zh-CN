---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b255c4ac0e5b284db533844f82a26dc50b07d701
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserDetail = await graphClient.Reports
    .GetOneDriveActivityUserDetail('D7')
    .Request()
    .GetAsync();

```