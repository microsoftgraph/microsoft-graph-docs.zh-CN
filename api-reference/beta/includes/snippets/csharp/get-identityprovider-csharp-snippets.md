---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6b353d82ea072ad6b6680bd9cc0b34e3cbafac5
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.IdentityProviders
    .Request()
    .GetAsync();

```