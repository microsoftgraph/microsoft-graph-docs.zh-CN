---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b83fe42abab128fea4456830c666bfc4f20b4e0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{event-id}"].Attachments["{attachment-id}"]
    .Request()
    .DeleteAsync();

```