---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14522f73701b02de345e06be6d46ba10213380c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793248"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Events["{event-id}"].Attachments["{attachment-id}"]
    .Request()
    .GetAsync();

```