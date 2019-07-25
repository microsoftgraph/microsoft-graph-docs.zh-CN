---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 02a8c0ce82175be422467ef9d9a86bd932eb24bb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettings = await graphClient.GroupSettings
    .Request()
    .GetAsync();

```