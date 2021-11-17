---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c584670171e3e4bafd0e630bd6041eb8d97ba7c455f8d73d403409a1b34d7e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRules = await graphClient.Me.MailFolders["{mailFolder-id}"].MessageRules
    .Request()
    .GetAsync();

```