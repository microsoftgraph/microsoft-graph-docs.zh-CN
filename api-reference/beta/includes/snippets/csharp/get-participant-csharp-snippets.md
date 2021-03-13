---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bd1b87408b304015b87c5cb88a3feaa87c5bcc7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participant = await graphClient.Communications.Calls["{call-id}"].Participants["{participant-id}"]
    .Request()
    .GetAsync();

```