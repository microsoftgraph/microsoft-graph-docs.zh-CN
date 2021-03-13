---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc90a53559c7d08ab5745f7b8c821885a91dbd99
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805044"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Sites["{site-id}"].Drive
    .Request()
    .GetAsync();

```