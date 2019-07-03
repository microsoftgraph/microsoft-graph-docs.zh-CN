---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e34080195ffe136a4eb99a120ce07e37f9900db6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessActivityUserDetail('D7')
    .Request()
    .GetAsync();

```