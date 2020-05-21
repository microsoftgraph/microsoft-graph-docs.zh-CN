---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec29c69ad56e51eec38dbeaa247e65bbf56f177d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Users["{id}"].MemberOf
    .Request()
    .GetAsync();

```