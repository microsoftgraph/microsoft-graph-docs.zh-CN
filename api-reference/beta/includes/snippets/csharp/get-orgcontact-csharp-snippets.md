---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b7d9875e8719bcefed2ac4c8ab16ebfd803a273
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["{orgContact-id}"]
    .Request()
    .GetAsync();

```