---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d32bf12cd6e29251d0434cb1c83c9fe70f9818ac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var relations = await graphClient.TermStore.Sets["{termStore.set-id}"].Relations
    .Request()
    .GetAsync();

```