---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0af9970630858b0b98527f1bfbb7194994fb3dd7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request()
    .GetAsync();

```