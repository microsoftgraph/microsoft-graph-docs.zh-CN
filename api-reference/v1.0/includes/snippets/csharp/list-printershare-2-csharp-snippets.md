---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 525846dc4ce8421ad1d97537d2d7bfc9e0f1160c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956250"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shares = await graphClient.Print.Printers["{printer-id}"].Shares
    .Request()
    .GetAsync();

```