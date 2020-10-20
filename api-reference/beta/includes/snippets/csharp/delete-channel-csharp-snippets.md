---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 690db678ce07c8b29957bc91a2d1150dc8ceecf8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606543"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Channels["{id}"]
    .Request()
    .DeleteAsync();

```