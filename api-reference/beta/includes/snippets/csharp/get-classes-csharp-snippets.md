---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 189aabf7420f5dbc5c03fcffbc5e69bb78fc6001
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Me.Classes
    .Request()
    .GetAsync();

```