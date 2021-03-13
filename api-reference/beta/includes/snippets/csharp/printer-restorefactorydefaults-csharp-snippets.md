---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bf554d26a5229bbb1739bf7d5481ceb5a711ccd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"]
    .RestoreFactoryDefaults()
    .Request()
    .PostAsync();

```