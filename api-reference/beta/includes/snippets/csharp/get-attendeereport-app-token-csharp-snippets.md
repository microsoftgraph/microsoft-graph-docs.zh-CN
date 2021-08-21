---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff69fa0a59c52abc783db258baf2eebf0b4aa1dace85371153aa21d2f267e82e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101383"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].AttendeeReport
    .Request()
    .GetAsync();

```