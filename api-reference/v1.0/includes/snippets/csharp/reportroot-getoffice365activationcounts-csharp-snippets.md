---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8891b6c3023ef5485b1865bf6dcdb0f722b96b8a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActivationCounts()
    .Request()
    .GetAsync();

```