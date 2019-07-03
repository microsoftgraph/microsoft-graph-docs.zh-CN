---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ed2bb061ef847d5cf854faa44ca94a936ae471f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = await graphClient.Applications["{id}"]
    .Request()
    .GetAsync();

```