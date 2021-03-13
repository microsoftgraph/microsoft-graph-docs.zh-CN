---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17e6b8abafe96a3ab802a9c791f803acfd7ae4fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroup = await graphClient.Me.Onenote.SectionGroups["{sectionGroup-id}"]
    .Request()
    .GetAsync();

```