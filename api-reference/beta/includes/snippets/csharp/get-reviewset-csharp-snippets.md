---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2874f5b4b23c15c446a9b35742c2e1444309ff92
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566299"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSet = await graphClient.Compliance.Ediscovery.Cases["6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d"].ReviewSets["0157910c-57ce-4e48-bd4b-90f3c88ca32e"]
    .Request()
    .GetAsync();

```