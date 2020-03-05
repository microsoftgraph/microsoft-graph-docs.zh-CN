---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec580d4f2a7455dcf2d65d13b96d4af8dd41c2a0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37998269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Languages["{id}"]
    .Request()
    .DeleteAsync();

```