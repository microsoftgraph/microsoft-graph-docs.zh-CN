---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dde4b89f6986fb698d8b14a79ba9a2eef6fc0cc0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Users["13019"]
    .Request()
    .DeleteAsync();

```