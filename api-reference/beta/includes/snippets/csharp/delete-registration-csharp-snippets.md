---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a53dae878bd7fe96ec626bd270e14ca27b1f7df
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration
    .Request()
    .DeleteAsync();

```