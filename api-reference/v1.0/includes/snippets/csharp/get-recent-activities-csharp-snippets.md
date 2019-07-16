---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bcaab345dffb05ab00cfda6bf015ac1a94bd2ce6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Activities.Recent()
    .Request()
    .GetAsync();

```