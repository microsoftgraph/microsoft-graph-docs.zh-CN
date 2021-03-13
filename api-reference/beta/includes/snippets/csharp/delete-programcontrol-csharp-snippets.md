---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba082a795f4b9cab158bb28b10b08c81a5711d49
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ProgramControls["{programControl-id}"]
    .Request()
    .DeleteAsync();

```