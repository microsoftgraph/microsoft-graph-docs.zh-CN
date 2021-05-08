---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1110c96cfb7592b7baf8b25eaffef36e5fcda0d9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241413"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entries = await graphClient.Admin.Windows.Updates.Catalog.Entries
    .Request()
    .GetAsync();

```