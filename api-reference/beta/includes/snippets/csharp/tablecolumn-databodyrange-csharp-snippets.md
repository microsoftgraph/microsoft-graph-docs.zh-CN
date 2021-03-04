---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1617cd9f59bb8b024d50e1fe2c5703054c48740a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .DataBodyRange()
    .Request()
    .GetAsync();

```