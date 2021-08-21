---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64331460fdcaf9801d17ae886e4fd8caeca84bd747707453af9b19f6b0e18e58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].Recording
    .Request()
    .GetAsync();

```