---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c679cd0fd8b2a952d0c85ebbb32127d9ee3acb6434aaed1aa757ee02ea51a7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161492"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tag = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Tags["{ediscovery.tag-id}"]
    .Request()
    .GetAsync();

```