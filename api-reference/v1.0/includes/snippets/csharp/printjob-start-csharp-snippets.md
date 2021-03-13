---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93da43d34adeb9cfafad56924893b2df95a45eab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Shares["{printerShare-id}"].Jobs["{printJob-id}"]
    .Start()
    .Request()
    .PostAsync();

```