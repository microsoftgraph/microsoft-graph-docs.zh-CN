---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 525846dc4ce8421ad1d97537d2d7bfc9e0f1160c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shares = await graphClient.Print.Printers["{printer-id}"].Shares
    .Request()
    .GetAsync();

```