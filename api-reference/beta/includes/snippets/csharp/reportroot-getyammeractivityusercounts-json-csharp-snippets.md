---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f4f76b3fe770413b516cca0ff20740ceb55256e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserCounts = await graphClient.Reports.GetYammerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```