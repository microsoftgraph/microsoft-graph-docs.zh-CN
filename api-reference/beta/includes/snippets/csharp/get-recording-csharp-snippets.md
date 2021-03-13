---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27ccc4a7b6162f5156c7bd5bbe037aa2fc2eecbf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795190"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].Recording
    .Request()
    .GetAsync();

```