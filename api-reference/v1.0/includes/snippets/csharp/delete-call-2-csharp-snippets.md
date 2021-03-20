---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b08bee508606ae08bdb70e191c47a4eb5e5f972
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"]
    .Request()
    .DeleteAsync();

```