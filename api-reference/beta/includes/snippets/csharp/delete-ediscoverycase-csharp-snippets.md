---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbe2f43d2c88728e5cd65a5e2f048cbfeb4608d7
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["061b9a92-8926-4bd9-b41d-abf35edc7583"]
    .Request()
    .DeleteAsync();

```