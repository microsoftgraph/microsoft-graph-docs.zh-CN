---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a52b317178c7c501d76b6c77ffffd9a91b45937f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageStorage = await graphClient.Reports.GetMailboxUsageStorage('D7')
    .Request()
    .GetAsync();

```