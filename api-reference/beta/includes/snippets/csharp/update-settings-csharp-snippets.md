---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d6ba6ae1080b7fa7a84e6fb135d63ba58954464
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948202"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printSettings = new PrintSettings
{
    DocumentConversionEnabled = true
};

var print = new Print();
print.Settings = settings;

await graphClient.Print
    .Request()
    .UpdateAsync(print);

```