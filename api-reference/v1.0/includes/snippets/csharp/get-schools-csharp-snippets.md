---
description: 自动生成的文件。 不修改
ms.openlocfilehash: adc7d16660ff7b459c7d0cb5fa2c1f58993b7076
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Me.Schools
    .Request()
    .GetAsync();

```