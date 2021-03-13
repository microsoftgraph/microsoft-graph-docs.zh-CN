---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d24176e8b1b9c7ad776ab63b145cd1a5559d6bf9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Onenote.Pages["{onenotePage-id}"]
    .Request()
    .DeleteAsync();

```