---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3a70709de9f72029c41592820408400597444b8
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35725645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timesOff = await graphClient.Teams["{teamId}"].Schedule.TimesOff
    .Request()
    .Filter("sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z")
    .GetAsync();

```