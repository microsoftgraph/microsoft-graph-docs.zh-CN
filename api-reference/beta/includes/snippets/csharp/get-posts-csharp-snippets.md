---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5362a54b861ab76cafe4ad723052e2e31ae7b176
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var posts = await graphClient.Groups["0d75b8dc-c42d-44dd-890a-751a99c0589f"].Threads["AAQkAD8EJUmcWwTJi06Cew=="].Posts
    .Request()
    .GetAsync();

```