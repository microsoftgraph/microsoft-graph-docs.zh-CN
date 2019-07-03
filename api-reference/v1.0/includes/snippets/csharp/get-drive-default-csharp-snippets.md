---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9702795737d7b370ed8999458513e984e0384904
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510259"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Me.Drive
    .Request()
    .GetAsync();

```