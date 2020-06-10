---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86de4386c0fd94466aaf71803244193c1d0ae1b4
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Directory.DeletedItems
    .Request()
    .GetAsync();

```