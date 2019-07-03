---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fba5222968d25e04bd53e804fe520a742dbda154
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRules = await graphClient.Me.MailFolders["inbox"].MessageRules
    .Request()
    .GetAsync();

```