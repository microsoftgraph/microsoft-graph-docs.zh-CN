---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a2136af5fae87c1a643ddd35a2cd670cd021915
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444550"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{itemId}"]
    .CreateLink(type,scope,expirationDateTime,password,message,recipients)
    .Request()
    .PostAsync();

```