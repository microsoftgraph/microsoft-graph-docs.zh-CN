---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ce9425c53c59749f14408f9bd03f37088c4eb0c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```