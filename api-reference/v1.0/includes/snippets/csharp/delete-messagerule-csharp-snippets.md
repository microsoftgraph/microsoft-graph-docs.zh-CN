---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4b68b4d2226680b60571465393ce8d46dcf724a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["inbox"].MessageRules["AQAAAJ5dZp8="]
    .Request()
    .DeleteAsync();

```