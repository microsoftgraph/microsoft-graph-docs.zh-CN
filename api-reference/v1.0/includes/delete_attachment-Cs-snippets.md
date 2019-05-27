---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f4bc03b863bb29eecdaef3a7fa8e9d15da15d8c9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"].Attachments["{id}"]
    .Request()
    .DeleteAsync();

```