---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 234f5efe9e638f705ced6ac50df8e778728511d4080ab7e350288a26eb5dfe3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.MailFolders
    .Delta()
    .Request()
    .GetAsync();

```