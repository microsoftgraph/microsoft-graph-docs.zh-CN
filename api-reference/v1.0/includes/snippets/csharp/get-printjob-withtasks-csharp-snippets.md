---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 719987cef1f13f8644b79080db070378975a4f81
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Request()
    .Expand("tasks")
    .GetAsync();

```