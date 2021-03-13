---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9e483602227aa1c36f0e22a3a572c27dcf14526
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sitePage = await graphClient.Sites["{site-id}"].Pages["{sitePage-id}"]
    .Request()
    .GetAsync();

```