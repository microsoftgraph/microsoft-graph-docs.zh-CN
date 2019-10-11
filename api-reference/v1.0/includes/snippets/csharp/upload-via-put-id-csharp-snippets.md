---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 035a1b352a5b8f7118b2ef79ec94854561b78159
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428863"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = "The contents of the file goes here."

await graphClient.Me.Drive.Items["{item-id}"].Content
    .Request()
    .PutAsync(stream);

```