---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d3f9f8f4b670bc4cd44b86437b4c844d999c645
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947661"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = await graphClient.Print.PrinterShares["{id}"]
    .Request()
    .GetAsync();

```