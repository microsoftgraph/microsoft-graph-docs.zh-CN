---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7d0ab1d66a2018982848b80fc799e7977b9ed1983463decba987dff13e148d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219451"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSet = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"]
    .Request()
    .GetAsync();

```