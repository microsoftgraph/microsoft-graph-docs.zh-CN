---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59c0f0920f72e71f813a4ca428e7f5531d1a6340
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947232"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reportRoot = await graphClient.Print.Reports["monthlyPrintUsageSummariesByUser"]
    .Request()
    .GetAsync();

```