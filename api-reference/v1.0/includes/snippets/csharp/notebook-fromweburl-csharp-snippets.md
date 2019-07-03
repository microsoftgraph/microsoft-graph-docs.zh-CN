---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ae4dbfc9a13d045a10ac95d38a6d6ea0b8ed7734
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493078"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webUrl = "webUrl value";

await graphClient.Me.Onenote.Notebooks
    .GetNotebookFromWebUrl(webUrl)
    .Request()
    .PostAsync();

```