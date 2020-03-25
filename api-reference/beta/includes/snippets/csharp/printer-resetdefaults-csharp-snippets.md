---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 084e70e5479fbda2738e7b085a0619ad083faf6b
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"]
    .ResetDefaults()
    .Request()
    .PostAsync();

```