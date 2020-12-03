---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdbc2244cec616d4010061612dd5bfa02d22bd9c
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49530646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationPrinterId = "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea";

await graphClient.Print.Printers["d5ef6ec4-07ca-4212-baf9-d45be126bfbb"].Jobs["44353"]
    .Redirect(destinationPrinterId,null)
    .Request()
    .PostAsync();

```