---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1541b331ef946860424fb6b943f88b2a23b818f2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{name}"].Children
    .Request()
    .GetAsync();

```