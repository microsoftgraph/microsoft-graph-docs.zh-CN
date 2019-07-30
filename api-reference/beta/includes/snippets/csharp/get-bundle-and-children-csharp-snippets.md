---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 098e967c3ced9f611448cb2833a2558ff03f2c5d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932663"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "children")
};

var driveItem = await graphClient.Drive.Items["{bundle-id}"]
    .Request( queryOptions )
    .GetAsync();

```