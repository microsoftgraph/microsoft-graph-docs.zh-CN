---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0287502a406a376da949102f62fecc183295c8a8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Directory.DeletedItems["46cc6179-19d0-473e-97ad-6ff84347bbbb"]
    .Request()
    .GetAsync();

```