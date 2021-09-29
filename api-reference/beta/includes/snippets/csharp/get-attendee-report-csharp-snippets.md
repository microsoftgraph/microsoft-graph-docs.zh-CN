---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4910c660b570689456f4e061fc5a610db347fb5
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendeeReport
    .Request()
    .GetAsync();

```