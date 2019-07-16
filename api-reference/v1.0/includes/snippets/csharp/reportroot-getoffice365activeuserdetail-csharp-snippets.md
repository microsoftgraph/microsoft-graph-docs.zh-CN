---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d1353d53391be008fbac1e5c367d71eec844357
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739435"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActiveUserDetail('D7')
    .Request()
    .GetAsync();

```