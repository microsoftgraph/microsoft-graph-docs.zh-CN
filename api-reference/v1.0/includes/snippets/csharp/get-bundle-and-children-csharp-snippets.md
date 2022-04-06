---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dc8721a190a2dbfc0248f456740190cb82cdca9
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "children")
};

var driveItem = await graphClient.Drive.Items["{driveItem-id}"]
    .Request( queryOptions )
    .GetAsync();

```