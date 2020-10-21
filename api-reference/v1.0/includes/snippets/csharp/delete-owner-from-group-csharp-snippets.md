---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a088a6281a80b7831e94744ac44b0e14622961b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```