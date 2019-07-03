---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c18a3e617e89748b6c11d1b8de81e664d6a8077e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var events = await graphClient.Groups["{id}"].Events
    .Request()
    .GetAsync();

```