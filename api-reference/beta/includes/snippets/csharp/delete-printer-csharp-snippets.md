---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4e2299ed39661b5f0916eca004e2b12862fce86
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .DeleteAsync();

```