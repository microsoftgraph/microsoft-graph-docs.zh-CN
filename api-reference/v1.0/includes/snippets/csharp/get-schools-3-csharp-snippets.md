---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adc7d16660ff7b459c7d0cb5fa2c1f58993b7076
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Me.Schools
    .Request()
    .GetAsync();

```