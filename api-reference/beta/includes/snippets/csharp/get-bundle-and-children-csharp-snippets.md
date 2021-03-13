---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dc8721a190a2dbfc0248f456740190cb82cdca9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784814"
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