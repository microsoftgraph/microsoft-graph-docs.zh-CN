---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b6aedb58e0074029bf3a788cd464e5f5d96a744
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .Range()
    .Request()
    .GetAsync();

```