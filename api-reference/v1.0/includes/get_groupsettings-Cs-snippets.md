---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 02a8c0ce82175be422467ef9d9a86bd932eb24bb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSettings = await graphClient.GroupSettings
    .Request()
    .GetAsync();

```