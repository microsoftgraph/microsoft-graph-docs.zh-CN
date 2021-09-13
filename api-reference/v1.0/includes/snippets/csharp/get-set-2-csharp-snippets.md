---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 721698c2e5cd09a95ee638ed8eedd0d00f375630
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"]
    .Request()
    .GetAsync();

```