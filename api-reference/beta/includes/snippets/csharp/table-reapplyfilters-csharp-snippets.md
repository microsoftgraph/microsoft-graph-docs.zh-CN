---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a30ec7733186ae4cd6c83ff0ebf4a842862c96cc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520674"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ReapplyFilters()
    .Request()
    .PostAsync();

```