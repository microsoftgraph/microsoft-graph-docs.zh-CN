---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28581bf182c4aa4120cf2b79d43d22473dd9639d
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330226"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var relations = await graphClient.TermStore.Sets["{setId}"].Relations
    .Request()
    .GetAsync();

```