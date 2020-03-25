---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07c38c9dcff7d046a970c8f3dc917910826cc6b6
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947891"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedUsers = await graphClient.Print.Printers["{id}"].AllowedUsers
    .Request()
    .GetAsync();

```