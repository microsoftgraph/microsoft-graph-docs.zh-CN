---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f382da9918ad373494f88086726a25776e7e700
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783411"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerCapabilities = await graphClient.Print.Printers["{printer-id}"]
    .GetCapabilities()
    .Request()
    .GetAsync();

```