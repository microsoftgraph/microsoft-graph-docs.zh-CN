---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf8cfe7136abbe7415c35cf4a19654c56d51afed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Anniversaries["{personAnnualEvent-id}"]
    .Request()
    .DeleteAsync();

```