---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17a1296557021e93c2403c705665c7417449fe2f
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.Organization["settings"].ProfileCardProperties["{id}"]
    .Request()
    .GetAsync();

```