---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b10775c563448dfd05b235e4bcab3de9aa68a3f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["1a5f91a7-9bd1-4d5f-bb86-f43554cac51c"].TaskTriggers["25be207e-1154-491f-aa68-a9f7007d4bec"]
    .Request()
    .DeleteAsync();

```