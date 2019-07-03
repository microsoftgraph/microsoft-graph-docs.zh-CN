---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0aab50285e7b65a8abc36358cc839276ff0f0f9b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509140"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Social events"
};

await graphClient.Me.Calendar
    .Request()
    .UpdateAsync(calendar);

```