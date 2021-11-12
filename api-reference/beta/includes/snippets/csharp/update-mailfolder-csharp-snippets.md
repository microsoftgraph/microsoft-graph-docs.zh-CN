---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c07a5c31b99466d19c7cdcc94181f8bc475a262b4cd67136294758bf2d8c310
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Request()
    .UpdateAsync(mailFolder);

```