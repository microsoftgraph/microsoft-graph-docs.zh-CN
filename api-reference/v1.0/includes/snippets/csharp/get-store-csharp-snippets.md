---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc5fc52868bb953a6b997223846c4ee6f9643e78
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var store = await graphClient.Sites["{site-id}"].TermStore
    .Request()
    .GetAsync();

```