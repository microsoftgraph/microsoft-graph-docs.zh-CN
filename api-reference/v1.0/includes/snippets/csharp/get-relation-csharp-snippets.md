---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9060a0c8baa025c7c77637d2be6996efd10ff2cd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var relations = await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Relations
    .Request()
    .GetAsync();

```