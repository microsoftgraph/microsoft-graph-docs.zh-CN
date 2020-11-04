---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7a0382cd35314a0a8eaac2918f0385548998854
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .TotalRowRange()
    .Request()
    .GetAsync();

```