---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d35818aa1492cf060b3365f4299f7066646e5e1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59015656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = new Microsoft.Graph.TermStore.Store
{
    DefaultLanguageTag = "en-US"
};

await graphClient.Sites["{site-id}"].TermStore
    .Request()
    .UpdateAsync(store);

```