---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6da7dc455c38733cabd6557caf832ad963b0b0dc
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationPrinterId = "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea";

await graphClient.Print.Printers["d5ef6ec4-07ca-4212-baf9-d45be126bfbb"].Jobs["44353"]
    .Redirect(destinationPrinterId)
    .Request()
    .PostAsync();

```