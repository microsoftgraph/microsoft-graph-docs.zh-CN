---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a318a89b64f83f81dadb5b1a8d26bbf764fe2f7
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.ServicePrincipals["{id}"].Owners
    .Request()
    .GetAsync();

```