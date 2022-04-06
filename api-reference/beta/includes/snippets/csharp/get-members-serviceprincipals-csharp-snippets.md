---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 513b295f1563cc9e2e74c75ffe1b847e3eaecae1
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516519"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = await graphClient.Groups["{group-id}"].Members
    .Request()
    .GetAsync();

```