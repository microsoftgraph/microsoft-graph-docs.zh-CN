---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48855693bd5e72a0ac4c41d1148369e11e45a04c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806368"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Request()
    .GetAsync();

```