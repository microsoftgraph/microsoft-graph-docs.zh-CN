---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b05810c6bce64f4395b45e6eb80bd642041beec
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948005"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = await graphClient.Print.Printers["{id}"]
    .Request()
    .GetAsync();

```