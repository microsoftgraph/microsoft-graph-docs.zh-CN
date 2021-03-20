---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d19af3e7398655e1ef5a78449db93db963f774a2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sets = await graphClient.TermStore.Groups["{termStore.group-id}"].Sets
    .Request()
    .GetAsync();

```