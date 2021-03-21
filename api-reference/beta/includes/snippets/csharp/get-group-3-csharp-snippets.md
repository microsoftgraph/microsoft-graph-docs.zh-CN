---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 881f159421f74f92667ccd43b2bd5686d131b840
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.TermStore.Groups["{termStore.group-id}"]
    .Request()
    .GetAsync();

```