---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b8515e2ae1bd170a18e5375c6bba60d97a7754e9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .GetAsync();

```