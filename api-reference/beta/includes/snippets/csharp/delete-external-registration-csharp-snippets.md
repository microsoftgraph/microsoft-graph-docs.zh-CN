---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a53dae878bd7fe96ec626bd270e14ca27b1f7df
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113582"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration
    .Request()
    .DeleteAsync();

```