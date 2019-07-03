---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8891b6c3023ef5485b1865bf6dcdb0f722b96b8a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActivationCounts()
    .Request()
    .GetAsync();

```