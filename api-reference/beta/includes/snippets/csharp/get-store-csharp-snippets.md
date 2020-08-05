---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03706001a0fa80548c08b2ec7fecc5c1b81f5830
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565811"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = await graphClient.TermStore
    .Request()
    .GetAsync();

```