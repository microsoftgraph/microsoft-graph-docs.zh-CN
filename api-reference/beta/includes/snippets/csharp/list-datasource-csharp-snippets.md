---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c457b02da2546de3f7d1f60f2ca010f89cd0498e
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239601"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataSource = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources["{ediscovery.noncustodialDataSource-id}"].DataSource
    .Request()
    .GetAsync();

```