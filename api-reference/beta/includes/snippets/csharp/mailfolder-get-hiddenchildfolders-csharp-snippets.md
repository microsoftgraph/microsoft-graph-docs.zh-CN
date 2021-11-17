---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1e87d4f6aea2fdb6503a1cd58b7b753e434b68eceb15149bc5cf21d2c90feca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328701"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("includeHiddenFolders", "true")
};

var childFolders = await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request( queryOptions )
    .GetAsync();

```