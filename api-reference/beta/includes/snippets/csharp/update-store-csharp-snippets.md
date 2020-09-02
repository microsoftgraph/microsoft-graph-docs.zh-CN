---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 225d593a09aca986f81ba3e9c488178aa525e3f9
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = new Store
{
    DefaultLanguageTag = "en-US"
};

await graphClient.TermStore
    .Request()
    .UpdateAsync(store);

```