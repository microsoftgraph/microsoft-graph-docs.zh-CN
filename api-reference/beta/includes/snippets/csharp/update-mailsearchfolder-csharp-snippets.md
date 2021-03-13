---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65ac6dbe9161df302b326de2a4f19e97e8269621
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailSearchFolder
{
    FilterQuery = "contains(subject, 'Analytics')"
};

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Request()
    .UpdateAsync(mailFolder);

```