---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78c2220cc18c191cbff4c86c3dc1d6cee6af6a49
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var devices = await graphClient.Devices
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("extensionAttributes/extensionAttribute1 eq 'BYOD-Device'")
    .GetAsync();

```