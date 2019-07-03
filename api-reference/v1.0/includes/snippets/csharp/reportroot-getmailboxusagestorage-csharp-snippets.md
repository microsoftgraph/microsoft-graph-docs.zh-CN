---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dd62d3ed08df707bb815c5c10c2dd81f13076f00
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetMailboxUsageStorage('D7')
    .Request()
    .GetAsync();

```