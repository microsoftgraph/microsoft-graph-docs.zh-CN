---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4b68b4d2226680b60571465393ce8d46dcf724a7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721408"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["inbox"].MessageRules["AQAAAJ5dZp8="]
    .Request()
    .DeleteAsync();

```