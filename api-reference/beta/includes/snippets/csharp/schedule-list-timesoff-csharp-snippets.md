---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32dc4c1d8a588a7635f4927f11f57cad3616f5d3c0ec869c16a5a26e9fc80583
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timesOff = await graphClient.Teams["{team-id}"].Schedule.TimesOff
    .Request()
    .Filter("sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z")
    .GetAsync();

```