---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc2642f3b409670c44d5b196870083f701c065fa
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentTypes = await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .Request()
    .GetAsync();

```