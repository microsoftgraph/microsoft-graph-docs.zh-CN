---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95f9482afdb4efb55b847f63fb91815ed7770fe8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877691"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Users["{id}"].Outlook.Tasks["{id}"].Attachments
    .Request()
    .GetAsync();

```