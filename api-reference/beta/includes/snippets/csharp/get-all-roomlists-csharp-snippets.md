---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb663f29bddb2eb7ba4d2241d1275630c8846dd27fe8e25fa1baa3e6c1ddcf61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220246"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roomlist = await graphClient.Places
    .Request()
    .GetAsync();

```