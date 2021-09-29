---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dcc19796436af90f7d32270957f116cdca9b37f0242ac96a15bf9ad573bc7e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106121"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"]
    .Request()
    .DeleteAsync();

```