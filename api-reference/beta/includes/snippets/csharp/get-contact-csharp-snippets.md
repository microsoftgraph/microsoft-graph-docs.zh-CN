---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68cb62e3c0449c12a6a316022de0bb9c065f9df2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804198"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = await graphClient.Me.Contacts["{contact-id}"]
    .Request()
    .GetAsync();

```