---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcbb464efc9dc04f4cc594d3da1744f355641495
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("includeHiddenFolders", "true")
};

var mailFolders = await graphClient.Me.MailFolders
    .Request( queryOptions )
    .GetAsync();

```