---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3537972c0d2256540fc4fe248ff2c0bf4b1a73d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"].TaskTriggers["{printTaskTrigger-id}"]
    .Request()
    .DeleteAsync();

```