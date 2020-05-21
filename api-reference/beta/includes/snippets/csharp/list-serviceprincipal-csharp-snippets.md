---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58719bc70e18e04387d63ce6b5c2ef86249c1186
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceprincipals = await graphClient.Serviceprincipals
    .Request()
    .GetAsync();

```