---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8ebddb2b8df29cae374af2258acaa4858fc4ec7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = await graphClient.Communications.Calls["{call-id}"].Participants
    .Request()
    .GetAsync();

```