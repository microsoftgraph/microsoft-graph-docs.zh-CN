---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a81417d4824a96ebfac2d3592abf74ac0ab7b5cb
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShares = await graphClient.Print.PrinterShares
    .Request()
    .GetAsync();

```