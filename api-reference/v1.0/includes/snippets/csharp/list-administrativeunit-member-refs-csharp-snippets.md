---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a20edd2377b17d92d84a1b210987814ea36cb39
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "66040921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"].Members.References
    .Request()
    .GetAsync();

```