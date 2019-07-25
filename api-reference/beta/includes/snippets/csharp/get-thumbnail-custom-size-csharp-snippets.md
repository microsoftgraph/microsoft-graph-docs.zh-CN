---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 49914b3bfbaf0cb9c492a50d5efb447e27ef49fe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706130"
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