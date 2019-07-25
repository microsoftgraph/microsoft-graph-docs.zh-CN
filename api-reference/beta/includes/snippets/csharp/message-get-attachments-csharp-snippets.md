---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff29bbad94daeb381a85f2507e65ef80eef93bf5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Messages["{id}"].Attachments
    .Request()
    .GetAsync();

```