---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 857c28ba01a84120f3baaa9c6c38f57bb6eaa64d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = await graphClient.Teams["{id}"]
    .Request()
    .GetAsync();

```