---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bc23cd3d5428fbd77a022a619c05dc57fbe0afc3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473272"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Teams["303d2c1c-f1c5-40ce-b68e-544343d7f42b"].Channels["19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"].Messages
    .Request()
    .GetAsync();

```