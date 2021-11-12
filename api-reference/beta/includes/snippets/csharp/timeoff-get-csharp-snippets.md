---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 780f7cb277a0a951eefc93c52ef608e13d817ea728e361c16cba1a39c6457a7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOff = await graphClient.Teams["{team-id}"].Schedule.TimesOff["{timeOff-id}"]
    .Request()
    .GetAsync();

```