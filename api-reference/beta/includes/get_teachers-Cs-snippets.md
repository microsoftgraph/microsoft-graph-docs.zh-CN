---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9095f2d2b7439d99c9c4d7834bd5416846a7e69f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teachers = await graphClient.Education.Classes["11023"].Teachers
    .Request()
    .GetAsync();

```