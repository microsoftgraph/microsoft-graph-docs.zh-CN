---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5240c924a2bea4e7f98b5b894348d775fb0653f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771671"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .DeleteAsync();

```