---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7dfbc7eccffb58b85c06b94ce4941992dff8a32
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .Range()
    .Request()
    .GetAsync();

```