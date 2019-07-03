---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 81cb511d07cb9f8079cc625eb4aab928c0ff0c6e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreements = await graphClient.Agreements
    .Request()
    .GetAsync();

```