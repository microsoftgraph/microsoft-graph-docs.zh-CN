---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3163bb012eac86e5f8b9393c6d157faa61935d3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = await graphClient.Sites["{site-id}"].TermStore.Groups["{termStore.group-id}"].Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .GetAsync();

```