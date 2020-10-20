---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc3e4d190cc84edc7be903228c5d9d8bb10cfb10
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Root
    .Request()
    .GetAsync();

```