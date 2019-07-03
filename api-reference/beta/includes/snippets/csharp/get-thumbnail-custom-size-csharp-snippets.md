---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 49914b3bfbaf0cb9c492a50d5efb447e27ef49fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "c300x400_Crop")
};

var thumbnails = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails
    .Request( queryOptions )
    .GetAsync();

```